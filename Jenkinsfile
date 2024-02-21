pipeline {
    agent any 

    stages {
        stage("Checkout") {
            steps {
                git url: 'https://github.com/vinaypro5/Business_Management_Project.git'
                echo '************** CHECK-OUT COMPLETED *******************'
            }
        }
        stage("Build") {
            steps {
                bat "mvn clean install"
                echo '**************######### BUILD DONE ########*******************'
            }
        }
        stage("Test") {
            steps {
                bat "mvn test"
                echo '************** TEST COMPLETED *******************'
            }
        }
        stage("Package") {
            steps {
                bat "mvn package"
                echo '************** PACKAGE DONE *******************'
            }
        }
    }
}
