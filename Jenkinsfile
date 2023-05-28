pipeline {
    agent any
 
    stages {
        stage('Build') {
            steps {
                bat 'docker build -t web-server .'
            }
        }
     
        stage('Deploy') {
            steps {
                bat 'docker run -itd -p 80:80 web-server'
            }
        }
    }
}

