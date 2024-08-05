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
                sh "dotnet build /src/WeatherForecastApi.ApiService/WeatherForecastApi.ApiService.csproj"
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
