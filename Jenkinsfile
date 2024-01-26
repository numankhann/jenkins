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
                sh '''
                //cd myapp
                //pip install -r requirements.txt
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                sh '''
                //cd myapp
                //python3 hello.py
                p//ython3 hello.py --name=Numan
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
