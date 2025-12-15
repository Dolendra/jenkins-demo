pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code already checked out by Jenkins'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build stage running"'
                sh 'ls -l'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Test stage running"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline SUCCESS 🎉'
        }
        failure {
            echo 'Pipeline FAILED ❌'
        }
    }
}
