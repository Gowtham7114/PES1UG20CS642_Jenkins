pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS642 PES1UG20CS642.cpp'
                build job: 'PES1UG20CS642-1'
            }
        }

        stage('Test') {
            steps {
                sh './PES1UG20CS642'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Success'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
