pipeline {
    agent any

    tools {
        maven "M3"
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                git 'https://github.com/vinaypro5/Business_Management_Project.git'
            }
        }

        stage('Build') {
            steps {
                // Build your project using Maven
                bat 'mvn clean test -e -X'

            }
        }

        // Add more stages as needed (e.g., test, deploy)
    }

    post {
        success {
            echo 'Pipeline succeeded! Add additional success actions here if needed.'
        }
        failure {
            echo 'Pipeline failed! Add additional failure actions here if needed.'
        }
    }
}

