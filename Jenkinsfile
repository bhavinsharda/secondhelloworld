pipeline {
    agent any
    environment {
        runport = '3000'
      }
    stages {
        stage('Build') {
            steps {
                bat 'npm start -- on "3000" '
            }
        }
        stage('Deploy') {
            steps {
                bat 'node app.js'
            }
        }  
    }
}
