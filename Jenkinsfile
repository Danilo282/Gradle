pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Checkout'){
             deleteDir()
               checkout scm
            }
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
