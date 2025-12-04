pipeline {
    agent any
 
    stages {
        stage('Checkout') {
            steps {
                git checkout "https://github.com/AnushaAkkena/POC3.git"
            }
        }
 
        stage('Maven Build') {
            steps {
                sh 'mvn clean package -DskipTests'
            }
        }
 
        stage('Docker Build') {
            steps {
                sh 'docker build -t firstproject:latest .'
            }
        }
 
        stage('Docker Run') {
            steps {
                sh '''
                    docker run -d --name myapp -p 80:8080 firstproject:latest
                '''
            }
        }
    }
}
