pipeline {
    agent any 
    stages {
        stage('Test') { 
            steps {
                sh "cd src/tests/WeatherForecastApi.IntegrationTests && dotnet test --no-restore --configuration Release"
            }
        }
    }
}
