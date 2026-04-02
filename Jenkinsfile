pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/nishi-077/my-first-repo.git',branch:'master'
            }
        }
         stage('Build Image') {
            steps{
               bat 'docker build -t myjen .'
            }
    }
      stage('Stop Old Containers') {
            steps{
               bat 'docker stop mycont || exit 0' 
                bat 'docker rm mycont || exit 0'
    }
}
         stage('Run Image-Containerize') {
            steps{
               bat 'docker run -d -p 7000:80 --name mycont myjen' 
    }
}
}
}
