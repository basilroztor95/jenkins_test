pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/basilroztor95/jenkins_test'
            }
        }
        stage('Build') {
            steps {
                sh './hello.sh'
            }
        }
    }
}
