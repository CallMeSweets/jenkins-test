pipeline {
  agent any
  tools {
      maven 'maven'
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
