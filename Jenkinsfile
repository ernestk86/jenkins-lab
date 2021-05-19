pipeline {
    agent any
    stages {        
        stage('Build') {
            steps {
                sh 'javac Hello.java'
            }
        }        
        stage('Execute') {
            steps {
                sh 'java Hello'
            }
        }
    }
    post {
        always {
            emailext body: 'A Test EMail', to: 'ernest.kim@cognizant.com', subject: 'Build triggered'
        }
    }
}
