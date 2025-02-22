pipeline {
    agent{
        label 'AGENT-1'
    }
    options{
        timeout(time: 10,units: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                script {
                    sh "echo this is build"
                    sh "sleep 10"
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
            deleteDir()
        }
        success {
            echo "This section runs only when the pipeline is successful"
        }
        failure {
            echo "This section runs when the pipeline fails"
        }
    }
}
