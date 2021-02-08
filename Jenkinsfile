pipeline {
  agent any
  tools {
      maven 'mymaven'
      jdk 'myjdk11'
  }
  stages {
    stage("build"){
      steps {
        mvn clean package
        echo 'building application...'
      }
    }
  }

}
