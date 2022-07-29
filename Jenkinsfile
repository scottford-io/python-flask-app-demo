pipeline {
    agent any
    stages {
        stage('Build Python Flask App Docker Image') {
            when {
                branch 'main'
            }
            steps {
                script {
                    app = docker.build("$DOCKER_HUB/python-flask-app-demo")
                }
            }
        }
    }
}