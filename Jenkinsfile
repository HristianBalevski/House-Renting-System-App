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
                script {
                    sh '/usr/local/share/dotnet/dotnet build right-first-time.sln --configuration Release'
                }
        }
        stage('Run tests') {
            steps {
                sh 'dotnet test --no-build --configuration Release'
            }
        }
    }
}
