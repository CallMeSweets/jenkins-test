pipeline {
  agent any
  tools {
      maven 'maven'
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
