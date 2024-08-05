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
                sh "./..."
                sh "dotnet restore"
                sh "dotnet build"
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
