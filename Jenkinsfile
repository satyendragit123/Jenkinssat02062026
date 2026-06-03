pipeline {
agent any
stages {

    stage('Git Checkout') {
        steps {
            echo 'Source code downloaded from GitHub'
        }
    }

    stage('Install Dependencies') {
        steps {
            sh 'pip3 install -r requirements.txt'
        }
    }

    stage('Run Application') {
        steps {
            sh 'python3 app.py'
        }
    }

}

}

