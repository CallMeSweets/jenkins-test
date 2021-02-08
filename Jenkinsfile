pipeline {
  agent any
  tools {
      maven 'maven'
      jdk 'openjdk-11'
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
