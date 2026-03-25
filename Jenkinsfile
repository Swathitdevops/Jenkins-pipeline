
pipeline {
    agent {
        label 'Docker-Slave'
    }

    environment {
        DOCKER_CREDS = credentials('Dockerhub')
         DOCKER_REPO = 'swathitdevops/nginx-image'
    }

    stages {
        stage('DockerBuildProcess') {
            steps {
                sh "docker pull nginx"
                sh "docker tag nginx ${DOCKER_REPO}:v1"
                sh "docker login -u ${DOCKER_CREDS_USR} -p ${DOCKER_CREDS_PSW}"
                sh "docker push ${DOCKER_REPO}:v1"
            }
        }
    }
}
