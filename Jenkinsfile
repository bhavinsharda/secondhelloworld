pipeline {
    agent any
    environment {
        runport = '3000'
      }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Deploy') {
            steps {
                runport
                bat 'node app.js'
            }
        }  
    }
}
