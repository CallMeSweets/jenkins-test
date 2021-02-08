pipeline {
  agent any
  tools {
      jdk 'jdk11'
  }
  stages {
    stage("build"){
      steps {
        echo 'maven version'
        sh 'mvn -version'
        echo 'building application...'
        sh 'mvn clean package'
      }
    }
  }
  post {
    success {
        echo 'building image...'
        sudo docker build -t message-service .
    }
    failure {
        echo 'building failure...'
    }
  }
}
