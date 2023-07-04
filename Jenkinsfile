pipeline {
    agent any

    stages {
        stage('build') {
            steps {
           
                echo 'Hello World'
                        
                sh """
                  docker build . -t -f Dockerfile nginx:latest 
                  
                """
           
            }
          }
        }
    }

