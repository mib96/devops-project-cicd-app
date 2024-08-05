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
                sh "cd /src/WeatherForecastApi.ApiService/"
                sh "dotnet build --configuration Release"
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploy' 
            }
        }
    }
}
