pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/yourusername/yourrepo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'  // If using Java & Maven
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'  // Run unit tests
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
                // Add deployment commands, e.g., copying files to IIS server
            }
        }
    }
}
