pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'dotnet build'
            }
        }

        stage('Run tests') {
            steps {
                sh 'dotnet test'
            }
        }
    }
}