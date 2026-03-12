pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                echo 'Cloning GitHub repository...'
                git 'https://github.com/Im-Gowtham9/sample-jenkins-project.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                echo 'Running tests...'
                sh 'pytest'
            }
        }

        stage('Build') {
            steps {
                echo 'Build successful!'
            }
        }
    }
}
