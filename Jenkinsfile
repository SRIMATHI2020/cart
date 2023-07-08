// Nodejs
pipeline {
    agent {label 'WS' }
    stages {           ///
        stage('Lint Checks') {
            steps {
              sh "echo Installing Jslint"
              sh "npm i jslint"
              sh "node_modules/jslint/bin/jslint.js server.js"
            }             /////
        }
    }
}