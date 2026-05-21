pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Cloning Source Code'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Application'
            }
        }

        stage('Docker Build') {
            steps {
                echo 'Creating Docker Image'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application'
            }
        }
    }
}
