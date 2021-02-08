pipeline {
  agent any
  tools {
      maven 'mymaven 3.6.3'
      jdk 'myjdk11'
  }
  stages {
    stage("build"){
      steps {
        sh 'mvn package'
        echo 'building application...'
      }
    }
  }

}
