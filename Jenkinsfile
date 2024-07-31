pipeline {
    agent any
    environment {
        PASSWORD = credentials('MB_CRED')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Build..'
                echo "Password is $PASSWORD"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
