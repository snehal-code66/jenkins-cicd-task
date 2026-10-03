
pipeline {
    agent any

    environment {
        PATH = "C:\\Users\\DELL\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin;${env.PATH}"
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building Docker image...'
                bat 'docker build -t my-web-app:latest .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Docker image...'
                bat 'docker image inspect my-web-app:latest'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Docker application...'
                bat 'docker rm -f my-web-container || exit /b 0'
                bat 'docker run -d --name my-web-container -p 8080:80 my-web-app:latest'
            }
        }
    }
}
