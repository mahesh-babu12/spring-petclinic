pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/mahesh-babu12/spring-petclinic.git'
            }
        }
        stage('Build') {
            steps {
                bat 'mvnw.cmd clean install'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}

