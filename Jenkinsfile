pipeline {
  agent any
  
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

