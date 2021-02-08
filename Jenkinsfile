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
        sh 'mvn clean package'
        echo 'building application...'
      }
    }
  }

}
