pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', 
                    url: 'https://github.com/codemaster170/test.git',
                    credentialsId: 'github-token'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}


