pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/nandanmayya-commits/portfolio.git'
            }
        }

        stage('Build with Maven') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

    }
}