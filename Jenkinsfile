pipeline {
    agent any

    stages {
        stage('Compile & Run Main') {
            steps {
                dir('src/main/java') {
                    // Bu blok içinde pwd = "workspace/src/main/java"
                    sh 'javac org/example/Main.java'
                    sh 'java org.example.Main'
                }
            }
        }
        stage('Compile & Run Main2') {
            steps {
                dir('src/main/java') {
                    sh 'javac org/example/Main2.java'
                    sh 'java org.example.Main2'
                }
            }
        }
    }
}
