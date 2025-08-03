pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Yash13raj13/node-js-sample.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run App') {
            steps {
                bat 'node app.js'
            }
        }
    }
}
