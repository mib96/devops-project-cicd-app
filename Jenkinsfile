pipeline {
    agent any 
    stages {
        stage('Test') { 
            steps {
                sh "dotnet test --no-restore --configuration Release"
            }
        }
    }
}
