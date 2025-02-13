pipeline {
    agent any 

    stages {
        stage('Restore dependencies') {
            steps {
                sh 'dotnet restore'
            }
        }
        stage('Build') {
            steps {
                sh 'dotnet build --configuration Release'
            }
        }
        stage('Run tests') {
            steps {
                sh 'dotnet test --no-build --configuration Release'
            }
        }
    }
}
