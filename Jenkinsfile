pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git credentialsId: 'your-credential-id', url: 'https://github.com/YOUR_USERNAME/jenkins-devsecops-pipeline.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'node index.js'
            }
        }
        stage('Test') {
            steps {
                echo 'Running Tests...'
                sh 'echo "No tests yet!"'
            }
        }
    }
}
