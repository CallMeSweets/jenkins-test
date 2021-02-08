pipeline {
  agent { docker { image 'maven 3.6.3' } }
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
