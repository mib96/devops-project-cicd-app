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
                sh "dotnet restore"
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
