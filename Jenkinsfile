pipeline {
    agent any
     tools {
        maven 'maven3'
    }
    stages {
        stage('checkout') {
            steps {
                git url: 'https://github.com/sdineshgandhi/k8s-demo-deploy1.git', branch: 'main'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }
        stage('build docker image'){
            steps{
                script {
                sh 'docker build -t sdineshgandhi/maven1:latest . '
                }
            }
        }
        stage('Docker push'){
            step{
                'sh '
            }
        }
    }
}