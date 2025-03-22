pipeline {
    agent any

    stages {
        stage('Project 1 - Compile & Run') {
            steps {
                sh 'javac Main.java'
                sh 'java Main'
            }
        }
        stage('Run') {
            steps {
                sh 'javac Main2.java'
                sh 'java Main2'
            }
        }
    }
}