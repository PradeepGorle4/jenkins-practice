pipeline {
    agent { label 'AGENT-1'}
    stages {
        stage('Build') {
            steps {
                script{
                    sh """
                    echo "Hello, this is build"
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

}