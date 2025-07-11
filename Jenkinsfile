pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t gruppenarbeit_dc:latest .'
            }
        }

        // stage('Deploy to DEV') {
        //     steps {
        //         sh 'kubectl apply -f deployment-kurs2-dev.yaml'
        //         sh 'kubectl apply -f service-kurs2-dev.yaml'
        //     }
        // }

        // stage('Deploy to PROD') {
        //     steps {
        //         sh 'kubectl apply -f deployment-kurs2-prod.yaml'
        //         sh 'kubectl apply -f service-kurs2-prod.yaml'
        //     }
        // }
    }
}
