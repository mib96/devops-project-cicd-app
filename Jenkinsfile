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
        stage('Publish') {
            steps {
                script {
                    sh """
                    cd src/
                    dotnet publish WeatherForecastApi.Web -c Release --output ./build_output
                    """
                }
            }
        }  
    }
}
