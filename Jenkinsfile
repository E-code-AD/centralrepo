pipeline {
  agent any
  stages {
    stage("run frontend") {
      steps {
        echo 'building the aplication ...'
        echo 'executing yarn'
        nodejs('Node-20-07') {
          sh 'yarn install'
        }
        
      }
    }
    stage("run backend") {
      steps {
        echo 'executing gradle'
        withGradle(){
          sh './gradlew -v'
        }
      }
    }
    
  }
}
