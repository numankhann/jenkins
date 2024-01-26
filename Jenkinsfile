pipeline {
    agent any
    triggers {
        pollSCM('* * * * *') // Polls the SCM each minute
    }

    stages {
        stage('Checkout') {
            steps {
                // Check out your Git repository
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }
}
