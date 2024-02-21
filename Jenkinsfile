pipeline {
    agent any 

    stages {
        stage("Checkout") {
            steps {
                git url: 'https://github.com/vinaypro5/Business_Management_Project.git'
            }
        }
        stage("Build") {
            steps {
                bat "mvn clean install"
            }
        }
        stage("Test") {
            steps {
                bat "mvn test"
            }
        }
        stage("Package") {
            steps {
                bat "mvn package"
            }
        }
    }
}
