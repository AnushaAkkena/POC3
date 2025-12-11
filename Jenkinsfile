pipeline {
    agent any
 
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/AnushaAkkena/POC3.git' , branch : 'main'
            }
        }
 
        stage('Maven Build') {
            steps {
                sh 'mvn clean package'
            }
        }
          stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
 
        stage('Docker Build') {
            steps {
                sh 'docker build -t project:latest .'
            }
        }
 
        stage('Docker Run') {
            steps {
                sh '''
                    docker run -d --name app -p 82:8080 project:latest
                '''
            }
        }
    }
}
