pipeline {
  agent none
   tools { 
        maven 'maven' 
        jdk 'jdk8' 
    }
  stages {
    stage('build initialization') {
      steps {
        step{
        echo 'This step is for compilation'
        sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
        }
      }
    }

  }
}
