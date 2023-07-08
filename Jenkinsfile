pipeline {
    agent any

    stages {
        stage('build') {
            steps {
           
                echo 'Hello World'
                withCredentials([usernamePassword(credentialsId: '390b8f5a-0950-4807-a2e7-3aea311de502', passwordVariable: 'password', usernameVariable: 'username')]) {
                sh "docker login -u $username -p $password "
}
           
            }
          }
        }
    }

