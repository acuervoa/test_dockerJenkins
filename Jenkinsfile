pipeline {
  agent {
    docker {
      image 'node:12'
      args '--network dockerjenkinspipeline_mynet'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

  }
}