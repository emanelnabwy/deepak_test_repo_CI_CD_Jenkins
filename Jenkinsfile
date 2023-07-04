pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'Hello World'
                //git 'https://github.com/emanelnabwy/deepak_test_repo_CI_CD_Jenkins.git'
                withCredentials([usernamePassword(credentialsId: 'emanelnabwy', usernameVariable: 'DOCKER_USERNAME', passwordVariable: 'DOCKER_PASSWORD')]) {
          
                // Login to Docker registry
              
          
                sh """
                  docker login -u ${DOCKER_USERNAME} -p ${DOCKER_PASSWORD}"
                  docker build . -t -f Dockerfile nginx:latest 
                  
                """
            }
            }
        }
    }
}
