pipeline {
    agent any
     options {
        disableRestartFromStage()
    }

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
         // Add a 15-second delay here
        stage('Wait 15 Seconds') {
            steps {
                echo 'Sleeping for 15 seconds...'
                sleep(15)
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
