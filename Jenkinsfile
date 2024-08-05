pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh """
                cd /src/WeatherForecastApi.ApiService/
                dotnet restore
            """
            }
        }
    }
}
