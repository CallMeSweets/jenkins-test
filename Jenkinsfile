pipeline {
  agent any
  environment {
   PATH = "/usr/share/maven/bin:$PATH"
  }
  tools {
      maven 'mymaven'
      jdk 'myjdk11'
  }
  stages {
    stage("build"){
      steps {
        echo 'java version'
        sh 'java -version'
        echo 'maven version'
        sh 'mvn -version'
        echo 'building application...'
      }
    }
  }

}
