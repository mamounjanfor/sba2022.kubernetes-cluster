pipeline {
      agent any
          stages {
               stage('Clone Repository') {
               steps {
               checkout scm
               }
          }
          stage('Build Image') {
               steps {
               sh 'sudo docker build -t 19841022/test3 .'
               }
         }
         stage('Run Image') {
               steps {
               sh 'sudo docker run -d --name myapptest 19841022/test3'
               }
         }
         stage('Testing') {
              steps {
                    echo 'Testing...'
                    }
         }
}
}  
