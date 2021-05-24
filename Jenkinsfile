pipeline {
  agent {
    docker {
      image 'gradle:jdk11'
    }

  }
  stages {
    stage('Say Hello') {
      steps {
        sh 'echo "Hello World"'
      }
    }

  }
}