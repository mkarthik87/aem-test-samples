pipeline {
  agent none
  stages {
    stage('build initialization') {
      agent {
        docker 'maven:3-alpine'
      }
      steps {
        sh 'mvn clean compile'
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