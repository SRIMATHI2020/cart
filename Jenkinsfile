@Library('Roboshop-shared-libary')

pipeline {
    agent { label 'WS' }
    stages {           ///
        stage('Lint Checks') {
            steps {
              script {
                 sample.info()
              }
              sh "echo Installing Jslint"
              sh "npm i jslint"
              sh "node_modules/jslint/bin/jslint.js server.js || true"
            }             /////
        }
        stage ('Code Compile') {
            steps{
                sh "npm install"
            }
        }
    }
}