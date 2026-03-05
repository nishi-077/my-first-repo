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
               bat 'javac jen1.java'
            }
        }
         stage('Execute') {
            steps {
                bat 'java jen1'
            }
        }
    }
}
