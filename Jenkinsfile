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
                sh '''
                    python3 -m venv venv
                    ./venv/bin/pip install -r requirements.txt
                '''
            }
        }
}
}

