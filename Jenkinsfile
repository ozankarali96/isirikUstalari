pipeline {
    agent any

    stages {
          stage('Clone repository') {
            steps {
                 cleanWs()
                          script {
                              git credentialsId: 'git-ozan', url: 'https://github.com/insiderqabootcampefinalproject/insiderbootcampproject-ozankarali96.git', branch: 'main'
                          }
                      }
                  }

        stage('Compile') {
            steps {
                // Main.java dosyasını derliyoruz.
                sh 'javac Main.java'
            }
        }
        stage('Run') {
            steps {
                // Derlenmiş sınıfı çalıştırıyoruz.
                sh 'java Main'
            }
        }
    }
}
