pipeline {
    environment {
        registry = "thesecureautomator/python-flask-app-demo"
        registryCredential = 'docker_hub'
        dockerImage = ''
    }
    agent any
    stages {
        stage('Build Python Flask App Docker Image') {
            steps {
                script {
                  dockerImage = docker.build registry + ":$BUILD_NUMBER"
                }
            }
        }
    }
}