pipeline {
    agent any
    environment {
        CRED = credentials('MB_CRED')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Build..'
                echo 'Password is $CRED'
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
