pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build..'
                echo 'Password is ${MB_CRED}
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
