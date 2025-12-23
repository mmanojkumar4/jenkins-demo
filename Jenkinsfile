
pipeline {
    agent any

    stages {
        stage('Good Stage') {
            steps {
                echo 'This stage will pass'
            }
        }

        stage('Failing Stage') {
            steps {
                bat 'echo wrongcommand'
            }
        }

        stage('Never Runs') {
            steps {
                echo 'You will not see this'
            }
        }
    }
}

