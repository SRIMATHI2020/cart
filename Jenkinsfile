// Nodejs
pipeline {
    agent {label 'WS' }
    stages {
        stage('Lint Checks') {
            steps {
              sh "echo Installing Jslint"
              sh "npm i jslint"
              sh "ls -ltr node_modules/bin/"
              sh "node_modules/jslint/bin/jslint.js server.js"

            }
        }
    }
}