pipeline {
    agent any

    environment {
        // Define any environment variables here if needed
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Vamaa-shah/jenkins-lab2.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add your deployment steps here
            }
        }

        // Comment out Notify stage to avoid SMTP connection errors
        /*
        stage('Notify') {
            steps {
                mail to: 'someone@example.com',
                     subject: "Pipeline: ${currentBuild.fullDisplayName}",
                     body: "Build result: ${currentBuild.currentResult}"
            }
        }
        */
    }
}
