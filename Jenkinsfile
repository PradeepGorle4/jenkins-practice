pipeline {
    agent { label 'AGENT-1'}
    environment {
        PROJECT = 'EXPENSE'
        COMPONENT = 'BACKEND'
    }
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                    echo "Hello, this is build"
                    echo "Project: $PROJECT"
                    """
                }
            }
        }
        stage('Test') {
            steps {
                script{
                    sh """
                    echo "Hello, this is test"
                    """
                }
            }
        }
        stage('Deploy') {
            steps {
                script{
                    sh """
                    echo "Hello, this is deploy"
                    """
                }
            }
        }
    }
    post {
        always {
            echo "I will always say hello-again"
        }
        failure {
            echo "I will run when pipeline fails"
        }
        success {
            echo "I will run when pipeline succeeds"
        }
    }
}