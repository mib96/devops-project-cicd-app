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
                    dotnet restore
                    dotnet build
                    """
                }
            }
        }
    }
}
