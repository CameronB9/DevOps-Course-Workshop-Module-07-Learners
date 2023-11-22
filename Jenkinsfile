pipeline {
    agent none
    stages {
        stage('dotnet') {
            agent {
                docker { image 'mcr.microsoft.com/dotnet/sdk:7.0' }
            }
            steps {
                sh 'dotnet -h'
            }
        }
    }
}