pipeline {
  agent any
  tools {
    Gradle-6.2
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
  }
  
  
}

