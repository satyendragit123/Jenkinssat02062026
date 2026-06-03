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
                sh 'pip3 install -r requirements.txt --break-system-packages'
            }
        }
        stage('Run Application') {
            steps {
                echo 'Dependencies installed successfully!'
                // If you want to run your Python app, uncomment the line below:
                // sh 'python3 app.py' 
            }
        }
    }
}
