Jenkinsfile
pipeline {
    agent any

    stages {

        stage ('Build Docker Image'){
            steps{
                script{
                    dockerapp = docker.Build("fernandocarlosantos/kube_news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }

}
