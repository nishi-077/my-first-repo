pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git "https://github.com/nishi-077/my-first-repo.git"
            }
        }
         stage('Publish') {
            steps{
                publishHTML([
                    allowMissing:true,
                    alwaysLinktToLastBuild:false,
                    keepAll:false,
                    reportDir:'.',
                    reportFiles:'jenhtml.html',
                    reportName:'My html Publish'
    ])
    }
    }
}
}
