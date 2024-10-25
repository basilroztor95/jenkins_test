pipeline {
        agent any
        stages {
                stage('Build') {
                        steps {
                                echo 'Building...'
                                sh 'echo "1" | sudo docker pull leonskottkennedy/testdocker'
                                sh 'echo "1" | sudo docker run -d -p 3000:3000 leonskottkennedy/testdocker:latest'
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
