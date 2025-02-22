pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh "echo this is build"
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh "echo this is test"
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh "echo this is deploy"
                }
            }
        }
    }
    post {
        always {
            echo "This section runs always"
        }
        success {
            echo "This section runs only when the pipeline is successful"
        }
        failure {
            echo "This section runs when the pipeline fails"
        }
    }
}
