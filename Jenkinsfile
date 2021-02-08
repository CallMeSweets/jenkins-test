pipeline {  
   agent any  
   tools {
      jdk 'jdk11'
   }
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
          sh 'docker build -t message-service .' 
       }  
   }  
}
