@Library('Roboshop-shared-libary') _

pipeline {
    agent { label 'WS' }
    stages {           ///
        stage('Lint Checks') {
            steps {
                   script {
                       nodejs.lintchecks()
                  }
            }         /////
        }
        stage ('Code Compile') {
            steps{
                sh "npm install"
            }
        }
    }
}