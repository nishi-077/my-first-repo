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
                    allowmissing:true,
                    alwaysLinktoLastBuild:false,
                    keepAll:false,
                    reportDir:'.',
                    reportFiles:'jenhtml.html',
                    reportName:'My html Publish'
    ])
    }
    }
}
}
