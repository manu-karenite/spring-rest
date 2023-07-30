pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub
                git 'https://github.com/manu-karenite/spring-rest.git'
            }
        }

        stage('Build') {
            steps {
                // Build your project (e.g., Maven build)
                sh 'mvn clean package --quiet'
            }
        }

        stage('Test') {
            steps {
                // Run tests (if applicable)
                sh 'mvn test'
            }
        }
    }
}
