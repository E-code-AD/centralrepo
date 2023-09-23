pipeline {
  agent any
  stages {
    stage("run frontend") {
      steps {
        echo 'building the aplication ...'
        echo 'executing yarn'
        nodejs('Node-20-07') {
          sh 'yarn install'
          sh 'npm install gradle --save-dev'
          
        }
        
      }
    }
    stage("run backend") {
      steps {
        echo 'executing gradle'
        withGradle(){
          sh './gradlew build'
        }
      }
    }
    
  }
}
