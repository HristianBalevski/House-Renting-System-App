pipeline {
    agent any 

    stages {
        stage('Restore dependecies') {
            steps{
                sh 'dotnet restore'
            }
        }
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