pipeline {
  agent any
  environment {
   PATH = "/usr/share/maven/bin:$PATH"
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
