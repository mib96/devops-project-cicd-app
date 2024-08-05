pipeline {
    agent any 
    stages {
        stage('Checkout') { 
            steps {
                checkout scm
            }
        }
        stage('Test') { 
            steps {
                git "https://github.com/mib96/devops-project-cicd-app.git"
                sh "dotnet restore"
                sh "dotnet run ./..."
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
