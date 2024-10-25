pipeline {
        agent any
        stages {
                stage('Build') {
                        steps {
                                echo 'Building...'
                                sh 'sudo docker pull leonskottkennedy/testdocker'
                                sh 'sudo docker run -d -p 3001:3000 leonskottkennedy/testdocker:latest'
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
