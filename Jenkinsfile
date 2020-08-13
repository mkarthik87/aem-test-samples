pipeline {
  agent none
  stages {
    stage('build initialization') {
      agent {
        docker 'maven:3-alpine'
      }
      steps {
        echo 'This step is for compilation'
        sh '''
              echo "PATH = ${PATH}"
              echo "M2_HOME = ${M2_HOME}"
              '''
      }
    }

  }
  post {
    success {
      echo 'Build success'
    }

    failure {
      echo 'Build failed'
    }

  }
}