pipeline {
    env.MYTOOL_VERSION = '3000'
    agent { 
        any 
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
