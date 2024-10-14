pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example build step
                sh 'make build' // or './gradlew build' for Gradle projects
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test step
                sh 'make test' // or './gradlew test' for Gradle projects
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Example deploy step
                sh 'make deploy' // or your custom deployment command
            }
        }
    }
}
