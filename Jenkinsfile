pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting code'
            }
        }

        stage('Build') {
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'

                sh '''
                mkdir -p /tmp/deployment
                cp app.py /tmp/deployment/

                echo "Deployment completed"
                '''
            }
        }
    }
}