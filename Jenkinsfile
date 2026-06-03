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
                echo 'Deploying application files to /opt/app...'
                // This copies all your repository files into the target directory
                sh 'cp -r . /opt/app/' 
            }
        }

    }
}
