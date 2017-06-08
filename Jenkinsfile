pipeline {
  agent any
  stages {
    stage('sample1') {
      steps {
        parallel(
          "sample1": {
            echo 'some'
            
          },
          "sample3": {
            echo 'hola'
            
          },
          "sample4": {
            echo 'hola'
            
          }
        )
      }
    }
    stage('sample2') {
      steps {
        echo 'test'
      }
    }
  }
}