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

  
  
}

