pipeline {
    agent any
    stages {
        stage('Build project') {
            when {
                branch 'feature-ci-pipeline' 
            }
            steps {
                bat 'dotnet build'
            }
        }
        
        stage('Execute tests') {
            when {
                branch 'feature-ci-pipeline' 
            }
            steps {
                bat 'dotnet test'
            }
        }        
    }
}
