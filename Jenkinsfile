pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo '===== Checking out code ====='
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo '===== Building application ====='
                echo 'npm install would run here'
            }
        }
        stage('Test') {
            steps {
                echo '===== Running tests ====='
                echo 'npm test would run here'
            }
        }
        stage('Deploy') {
            steps {
                echo '===== Deploying application ====='
                echo 'Deployment successful!'
            }
        }
    }
    
    post {
        success {
            echo '===== Pipeline completed successfully! ====='
        }
        failure {
            echo '===== Pipeline failed! ====='
        }
    }
}
