pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                script {
                    sh "cd src/WeatherForecastApi.ApiService && dotnet restore"
                    sh "dotnet build --configuration Release"
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh "dotnet test --no-restore --configuration Release"
                }
            }
        }
    }
}
