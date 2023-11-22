pipeline {
    agent none
    stages {
        stage('dotnet') {
            agent {
                docker { image 'mcr.microsoft.com/dotnet/sdk:7.0' }
            }
            environment {
                DOTNET_CLI_HOME = '/tmp/dotnet_cli_home'
                XDG_DATA_HOME = '/tmp'
            }
            steps {
                sh 'dotnet -h'
            }
        }
    }
}