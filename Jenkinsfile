pipeline {

    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/YOUR-USERNAME/YOUR-REPO.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }

    }

    post {

        success {
            echo 'All tests passed successfully!'
        }

        failure {
            echo 'Tests failed!'
        }

    }
}
