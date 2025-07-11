pipeline {
    agent any

    stages {
        stage('Docker Build') {
            steps {
                sh 'docker build -t gruppenarbeit_dc:latest .'
            }
        }

        stage('Deploy DEV') {
            steps {
                sh 'kubectl apply -f deployment-kurs2-dev.yaml'
                sh 'kubectl apply -f service-kurs2-dev.yaml'
            }
        }

        stage('Deploy PROD') {
            steps {
                sh 'kubectl apply -f deployment-kurs2-prod.yaml'
                sh 'kubectl apply -f service-kurs2-prod.yaml'
            }
        }
    }
}
