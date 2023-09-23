pipeline {
  agent any
  tools {
    gradle 'Gradle-6.2'
  }
  stages {
    stage("run fronend") {
      steps {
        echo 'executing yarn'
        nodejs('Node-20-07') {
          sh 'yarn install'
        }
      }
    }
    stage("run fbackend") {
      steps {
        echo 'executing yarn'
        
          sh './gradlew -v'
        
      }
    }
  }
  
  
}

