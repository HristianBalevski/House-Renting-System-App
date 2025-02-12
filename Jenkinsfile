pipeline {
    agent any
    stages {
        steps('Build') {
            sh 'dotnet build'
        }

        steps('Run Tests') {
            sh 'dotnet test'
        }
    }
}