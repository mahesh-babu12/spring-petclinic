pipeline {
    agent any

    stage('Checkout') {
    steps {
        git branch: 'main', url: 'https://github.com/mahesh-babu12/spring-petclinic.git'
    }
}

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
