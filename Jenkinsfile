pipeline {
    agent any

    environment {
        IMAGE = "rahulguthi/devops-app:v1"
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/rahulguthi033-tech/end-to-end-devops-project'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t $IMAGE .'
            }
        }

        stage('Push') {
            steps {
                sh 'docker push $IMAGE'
            }
        }

        stage('Deploy') {
            steps {
                sh 'kubectl apply -f k8s/'
            }
        }
    }
}
