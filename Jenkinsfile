pipeline {
    agent { 
        any {
            ENV_VARIABLE ''
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Deploy') {
            steps {
                bat 'node app.js'
            }
        }  
    }
}
