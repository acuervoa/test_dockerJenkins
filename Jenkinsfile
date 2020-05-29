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
        sh 'cd ./example_react; npm install'
      }
    }

    stage('Test') {
      steps {
        sh 'cd ./example-react; npm run test -- --coverage --watchAll=false'
      }
    }

  }
}