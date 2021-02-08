pipeline {  
   agent any  
   stages {  
       stage('build') {  
           steps {  
              echo 'maven version'
              sh 'mvn -version'
              echo 'building application...'
              sh 'mvn clean package'
           }  
       }  
   }  
   post {  
       always {  
         echo 'This will always run'  
       }  
       success {  
          echo 'building image...'
          sudo docker build -t message-service . 
       }  
       failure {  
          echo 'building failure...'
       }  
   }  
}
