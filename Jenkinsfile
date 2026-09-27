pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "Build stage started"'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Test stage started"'
            }
        }

        stage('Verify Repository') {
            steps {
                sh 'echo "Files in Jenkins workspace:"'
                sh 'pwd'
                sh 'ls -la'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}
