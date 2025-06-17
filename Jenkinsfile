pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building app..."'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
        stage('SonarQube Analysis') {
            steps {
                withSonarQubeEnv('SonarQubeServer') {
                    sh 'sonar-scanner'
                }
            }
        }
        stage('Snyk Scan') {
            steps {
                sh 'snyk test'
            }
        }
    }
}