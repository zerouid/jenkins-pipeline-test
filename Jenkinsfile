pipeline {
  agent none
  stages {
    stage('test') {
      agent {
        docker {
            image 'artifactory.blackline.corp/cargo/bl-build-node:14.13.1-alpine3.12'
            label 'linux'
            registryCredentialsId 'b0a50339-b337-4cb0-bc69-6c322fa95088'
            registryUrl 'https://artifactory.blackline.corp/cargo/'
            reuseNode true
        }
      }
      steps {
        sh 'uname -a'
      }
    }

  }
}
