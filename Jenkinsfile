pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git "https://github.com/nishi-077/my-first-repo.git"
            }
        }
         stage('Build') {
            steps {
               echo "Building application"
               bat 'javac fifth.java'
            }
        }
         stage('Deploy') {
            steps {
                echo "Deploying application"
                bat 'java fifth'
            }
        }
    }
}
