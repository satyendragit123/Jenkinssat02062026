pipeline {
    agent any

    tools {
        jdk 'JDK21'
        maven 'Maven3'
    }

    stages {

        stage('Git Checkout') {
            steps {
                echo 'Source code downloaded from GitHub'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Tests'
            }
        }

    }
}
