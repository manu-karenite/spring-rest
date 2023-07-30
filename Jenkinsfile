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
                echo "----------Resolving Maven Dependencies----------"
                sh 'mvn dependency:resolve --quiet'
                echo ""

                echo "----------Building Maven Project----------"
                sh 'mvn clean package --quiet'
                echo ""
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
