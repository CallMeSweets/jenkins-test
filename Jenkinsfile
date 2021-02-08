pipeline {
  agent any
  tools {
      maven 'maven 3.8'
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
