pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS642.cpp'
                sh 'g++ -o PES1UG20CS642 PES1UG20CS642.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                echo 'Test stage executed successfulllllly'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed Successfulllllly'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
