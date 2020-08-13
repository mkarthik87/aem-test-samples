pipeline {
  agent none
   tools { 
        maven 'Maven 3.6.3' 
        jdk8 'jdk8' 
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
