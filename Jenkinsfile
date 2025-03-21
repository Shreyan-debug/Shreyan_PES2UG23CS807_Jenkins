pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script { PES2UG23CS807-1
                    sh 'g++ -o hello_exec main/hello.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './hello_exec'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline Failed'
        }
    }
}
