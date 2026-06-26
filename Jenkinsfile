pipeline {
    agent any

    environment {
        DOCKER_REPO = "shubh010701/online_shopping_app"
        DOCKER_HUB_CREDS = 'docker-hub-credentials-id' 
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/Shubham-Srivastava07/online-shopping-portal.git'
            }
        }

        stage('Build Image') {
            steps {
                sh "docker build -t ${DOCKER_REPO}:${BUILD_NUMBER} ."
                sh "docker build -t ${DOCKER_REPO}:latest ."
            }
        }

        stage('Push to Docker Hub') {
            steps {
                withCredentials([usernamePassword(credentialsId: "${DOCKER_HUB_CREDS}", usernameVariable: 'USER', passwordVariable: 'PASS')]) {
                    sh "echo ${PASS} | docker login -u ${USER} --password-stdin"
                    sh "docker push ${DOCKER_REPO}:${BUILD_NUMBER}"
                    sh "docker push ${DOCKER_REPO}:latest"
                }
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker compose down --remove-orphans'
                sh 'docker compose up -d --build --force-recreate'
            }
        } 
    }
}
