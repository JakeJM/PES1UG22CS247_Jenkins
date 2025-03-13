pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ test.cpp -o test'
                echo 'Build successfull'
            }
        }
        stage('Test') {
            steps {
                sh './test'
                echo 'Test successfull'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment Stage:Nothing to be done'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
