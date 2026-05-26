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

    }

}
