pipeline {
  agent any
  tools {
      maven 'Maven 3.6.3'
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
