pipeline {
    agent any

    triggers {
        // This tells Jenkins to listen for GitHub push events
        githubPush()
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                // Example: run a build command
                sh 'echo Build success!'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                // Example test command
                sh 'echo Tests passed!'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }
    }
}
