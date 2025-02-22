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

        post {
        always{
            echo "This sections runs always"
            
        }
        succes{
            echo "this section runsonly hen pipeline successful"

        }
        failure{
            echo "fails when pipeline fails"
        }
    }
}
