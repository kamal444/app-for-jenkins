pipeline {
    agent {
        docker {
            image 'python:latest'
            args '-v /tmp:/tmp'
        }
    }

    stages {
        stage('1-Build') {
            steps {
                echo 'Start Build'
                echo 'Building'
                echo 'End Build'
            }
        }
        stage('2-Test') {
            steps{
                echo 'Start Test'
                echo 'Testing'
                sh 'ls -la'
                echo 'End Test'
            }
        }
        stage('3-Deploy'){
            steps{
                echo 'Start Deploy'
                echo 'Deploying'
                sh '''
                    echo 'Line-1'
                    echo 'Line-2'
                '''
                sh 'python --version'
                echo 'End Deploy'
            }
        }
    }
}
