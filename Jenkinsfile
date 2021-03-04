pipeline {
  agent any
  stages {
    stage('') {
      agent {
        docker {
          image 'artifactory.blackline.corp/cargo/bl-build-node:14.13.1-alpine3.12\''
        }

      }
      steps {
        sh 'uname -a'
      }
    }

  }
}