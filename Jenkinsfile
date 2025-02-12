pipeline {
    agent any
    stages {
        stage('Build') {
            sh 'dotnet build'
        }

        stage('Run Tests') {
            sh 'dotnet test'
        }
    }
}