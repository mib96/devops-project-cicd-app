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
                    sh """
                    cd src/WeatherForecastApi.ApiService
                    dotnet build
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh """
                    cd src/tests/WeatherForecastApi.IntegrationTests
                    dotnet test
                    """
                }
            }
        }    
    }
}
