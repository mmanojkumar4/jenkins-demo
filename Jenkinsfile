pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checked out from GitHub'
            }
        }

        stage('Read README') {
            steps {
                bat 'type README.md'
            }
        }

        stage('Create Output') {
            steps {
                bat 'echo Pipeline from GitHub > output.txt'
            }
        }
    }
}
