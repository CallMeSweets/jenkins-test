pipeline {
  agent any
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
