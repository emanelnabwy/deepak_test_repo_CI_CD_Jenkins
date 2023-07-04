pipeline {
    agent any

    stages {
        stage('build') {
            steps {
           
                echo 'Hello World'
                        
                sh """
                  docker build . -f Dockerfile -t nginx:latest 
                  
                """
           
            }
          }
        }
    }

