pipeline {
    agent any
    stages {        
        //stage('git checkout') {
        //    steps {
        //        git 'https://github.com/ernestk86/jenkins-lab.git'
        //    }
        //}
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
}
