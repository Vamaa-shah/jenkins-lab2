pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Vamaa-shah/jenkins-lab2.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }

        stage('Notify') {
            steps {
                mail to: 'your-email@conestogac.on.ca',
                     subject: 'Jenkins Build Notification',
                     body: "Build completed: ${env.BUILD_URL}"
            }
        }
    }
}
