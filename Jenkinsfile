pipeline {
    agent any

    environment {
        NODE_ENV = 'development'
    }

    stages {
        stage('Checkout') {
            steps {
                git(
                    url: 'https://github.com/Yash13raj13/node-js-sample.git',
                    branch: 'master',
                    credentialsId: 'github-creds' // This is your GitHub PAT credential ID
                )
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                echo 'Starting application...'
                sh 'node app.js'
            }
        }
    }
}
