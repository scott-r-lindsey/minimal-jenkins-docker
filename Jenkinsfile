pipeline {
    environment {
        SERVICENAME     = 'minimal-jenkins-docker'
    }
    agent {
        docker {
            image 'node:10.16'
            args '-u root:root'
        }
    }
    stages {
        stage('Setup') {
            steps {
                sh 'echo "hello world"'
                sh 'whoami'
            }
        }
    }
}
