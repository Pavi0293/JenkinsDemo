pipeline {
    agent any

    stages {
        stage('Both build and test') {
            steps {
                parallel(
                    'Build': {
                        // All steps for the 'Build' branch go here
                        echo 'This is the Build stage'
                        sleep 15 // This is an example to show the delay from your image
                        // Example build command: sh 'mvn clean install'
                    },
                    'Test': {
                        // All steps for the 'Test' branch go here
                        echo 'This is the Test stage'
                        // Example test command: sh 'npm test'
                    }
                )
            }
        }
        
        // This is a sequential stage that will run after both parallel stages are complete
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
