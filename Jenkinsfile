pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                // The SCM configuration in Jenkins handles the checkout automatically
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                // You would put your build command here, e.g., `sh 'npm install'` or `sh 'mvn clean install'`
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // You would put your test command here, e.g., `sh 'npm test'` or `sh 'mvn test'`
            }
        }
    }
}
