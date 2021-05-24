pipeline {
  agent {
    docker {
      image 'gradle:jdk11'
    }

  }
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            sh 'echo "Hello World"'
          }
        }

        stage('') {
          agent {
            docker {
              image 'gradle:6.8.3-jdk'
            }

          }
          steps {
            sh 'ci/build-app.sh'
          }
        }

      }
    }

  }
}