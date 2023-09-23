pipeline {
  agent any
  
    tools {
        gradle 8.1 
    }
    stages {        
        stage('Build Image') {
            steps {
                sh 'gradle init'
                sh "echo 'building..'"
                
                withGradle {
                   sh 'gradle wrapper build'
                }
                
            }
        }

  
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
    
    
  }
}

