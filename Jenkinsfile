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
                bat "dotnet restore"
                bat "dotnet build --configuration Release"
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
