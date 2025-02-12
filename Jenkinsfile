pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '/Library/Frameworks/Mono.framework/Versions/Current/Commands/msbuild'
            }
        }

        stage('Run tests') {
            steps {
                sh 'dotnet test'
            }
        }
    }
}