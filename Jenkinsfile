pipeline {
    agent any 
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo Installing JSlist"
                sh "npm i jslint"
                sh "echo starting lintChecks ....."
                sh "node_modules/jslint/bin/jslint.js server.js || true"
                sh "echo linkChecks completed"
            }
        }
        stage('Generating Artifacts') {
            steps {
                sh "echo Generating Artifacts...."
                sh "npm install && ls -ltr"

            }
        }
    }
}