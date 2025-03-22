pipeline {
     agent any

     stages {
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