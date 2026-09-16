pipeline {
  agent {
    docker {
      image 'python:3.12-slim'
    }
  }

  stages {
    stage('Run Python') {
      steps {
        sh 'python app.py'
      }
    }
  }
}
