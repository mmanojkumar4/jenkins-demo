
// pipeline {
//     agent any

//     stages {
//         stage('Good Stage') {
//             steps {
//                 echo 'This stage will pass'
//             }
//         }

//         stage('Failing Stage') {
//             steps {
//                 bat 'echo wrongcommand'
//             }
//         }

//         stage('Never Runs') {
//             steps {
//                 echo 'You will not see this'
//             }
//         }
//     }
// }



pipeline {
    agent any

    stages {
        stage('Create Output') {
            steps {
                bat 'echo Pipeline artifact demo > pipeline-output.txt'
                bat 'echo Build Number: %BUILD_NUMBER% >> pipeline-output.txt'
            }
        }
    }

    post {
        success {
            archiveArtifacts artifacts: 'pipeline-output.txt'
        }
    }
}

