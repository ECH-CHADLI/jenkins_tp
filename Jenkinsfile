pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/ECH-CHADLI/jenkins_tp.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                bat 'javac HelloWorld.java'
                bat 'javac Merci.java'
                bat 'javac DeRien.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java HelloWorld'
                bat 'java Merci'
                bat 'java DeRien'
            }
        }
    }
}
