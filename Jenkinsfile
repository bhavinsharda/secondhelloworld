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
                runport = '3000'
                bat 'node app.js'
            }
        }  
    }
}
