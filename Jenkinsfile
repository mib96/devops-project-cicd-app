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
                sh "dotnet build /devops-project-cicd-app/src/WeatherForecastApi.ApiService"
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
