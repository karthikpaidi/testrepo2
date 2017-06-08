pipeline {
  agent any
  stages {
    stage('sample1') {
      steps {
        parallel(
          "A": {
            echo 'some'
            
          },
          "E": {
            echo 'hola'
            
          },
          "C": {
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
