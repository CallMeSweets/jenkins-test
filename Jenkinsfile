pipeline {
  agent any
  environment {
    JAVA_HOME = "/usr/lib/jvm/java-1.11.0-openjdk-amd64"
  }
  tools {
      maven 'Maven3'
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
