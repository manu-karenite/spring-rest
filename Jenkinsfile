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
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                // Run tests (if applicable)
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy your application (e.g., to a server)
                // Add deployment steps here
            }
        }
    }
}
