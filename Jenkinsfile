pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
			sh './hello.sh'
			sh 'mv index.html /var/www/html/'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
