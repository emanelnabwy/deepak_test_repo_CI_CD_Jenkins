pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                script {
                echo 'Hello World'
                withDockerRegistry([credentialsId: 'docker', url: '']) {         
                sh """
                  docker build . -t -f Dockerfile nginx:latest 
                  
                """
            }
            }
            }
          }
        }
    }

