node {
    agent any
      stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
          stage('test') {
            steps {
                bat 'npm deploy on --"3000"'
            }
        }
        stage('Deploy') {
            steps {
                bat 'node app.js'
            }
        }  
    }
}
