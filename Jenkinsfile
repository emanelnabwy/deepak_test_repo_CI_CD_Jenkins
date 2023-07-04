pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Hello World'
                //git 'https://github.com/emanelnabwy/deepak_test_repo_CI_CD_Jenkins.git'
                //withCredentials([SSH Username with private key(credentialsId: 'docker', usernameVariable: 'DOCKER_USERNAME', passwordVariable: 'DOCKER_PASSWORD')]) {
          
                // Login to Docker registry
              
          
                sh """
                  usermod -aG docker $USER
                  docker login -u emanelnabwy -p Kofta888!@#
                  docker build . -t -f Dockerfile nginx:latest 
                  
                """
            }         
          }
        }
    }

