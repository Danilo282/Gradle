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
    }
}


