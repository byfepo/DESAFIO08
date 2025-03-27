pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code..'
                git branch: 'master', url: 'https://github.com/byfepo/DESAFIO08.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the app..'
                sh 'npm install' // Ensure dependencies are installed
          }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the app..'
                script {
                    // Build the Docker image (assumes Dockerfile is in root)
                    docker.build('desafio08grupo02:latest')
                    // Alternative with more control:
                    // docker.build("your-image-name", "--file ./path/to/Dockerfile .")
                }
            }
        }
    }
}

