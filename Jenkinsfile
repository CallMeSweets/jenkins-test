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
}
