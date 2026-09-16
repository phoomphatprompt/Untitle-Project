pipeline {
  agent any

  environment {
    APP_NAME = 'Hello Jenkins App'
    ENVIRONMENT = 'development'
  }

  stages {
    stage('Show Build Information') {
      steps {
        echo "Application: ${APP_NAME}"
        echo "Environment: ${ENVIRONMENT}"
        echo "Build number: ${BUILD_NUMBER}"
        echo "Job name: ${JOB_NAME}"
        echo "Workspace: ${WORKSPACE}"
      }
    }

    stage('Build') {
      steps {
        echo "Building ${APP_NAME} for ${ENVIRONMENT}..."
        sh 'echo Build completed'
      }
    }
  }

  post {
    success {
      echo "Build #${BUILD_NUMBER} completed successfully."
    }

    always {
      echo 'Pipeline has finished.'
    }
  }
}
