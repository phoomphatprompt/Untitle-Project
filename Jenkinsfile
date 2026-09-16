pipeline {
  agent any

  stages {
    stage('Hello Jenkins') {
      steps {
        echo 'Hello World from Jenkins!'
      }
    }

    stage('Show Environment') {
      steps {
        sh 'echo Running on Jenkins'
        sh 'pwd'
      }
    }
  }
}
