pipeline {
  agent any
  tools {
      maven 'mavenxx'
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
