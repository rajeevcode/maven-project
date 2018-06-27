pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy to Staging') {
            steps {
                build job:'Deploy-to-staging'
                echo 'Deploying....'
            }
        }
    }
}