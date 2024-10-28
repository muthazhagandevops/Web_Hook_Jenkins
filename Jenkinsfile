pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git credentialsId: 'your-credentials-id', url: 'https://github.com/username/my-simple-app.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example build command
                sh 'echo "Simulating build process."'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
                sh 'echo "Simulating test process."'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please check the logs.'
        }
    }
}
