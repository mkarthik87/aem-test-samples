pipeline {
  agent any
  stages {
    stage('build initialization') {
      steps {
        echo 'This step is for compilation'
        sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
      }
    }

  }
  tools {
    maven 'maven'
    jdk 'jdk8'
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