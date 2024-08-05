pipeline {
    agent any 
    stages {
        stage('Test') { 
            steps {
                sh "cd src/WeatherForecastApi.ApiService && dotnet restore"
            }
        }
    }
}
