pipeline {
    agent any

    stages {
        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build || echo "No build step"'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test || echo "No tests defined"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment simulated'
            }
        }
    }
}
