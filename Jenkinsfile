pipeline {
    agent none
    stages {
        stage('dotnet') {
            agent {
                docker: { image: 'mcr.microsoft.com/dotnet/sdk:8.0' }
            }
            steps {
                sh 'dotnet -h'
            }
        }
    }
}