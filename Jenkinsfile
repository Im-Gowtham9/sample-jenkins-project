pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                bat python -m pip install -r requirements.txt
            }
        }

        stage('Run Tests') {
            steps {
                echo 'Running tests...'
                bat 'pytest'
            }
        }

        stage('Build') {
            steps {
                echo 'Build successful!'
            }
        }
    }
}
