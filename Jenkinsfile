pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
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
        stage ('Checkout'){
             deleteDir()
                 checkout scm
            }
        stage ('Build & Archive Apk') {
            sh 'export ANDROID_SERIAL=192.168.57.101:5555 ; ./build.sh'
               step([$class: 'ArtifactArchiver', artifacts: 'meu_aplicativo/build/outputs/apk/meu_aplicativo.apk'])
            }
         }
       }




