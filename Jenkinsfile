pipeline {
  agent any
  
    
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
  
}

