pipeline {
  agent any
  stages {
    stage('sample1') {
      steps {
        parallel(
          "A": {
            echo 'some'
            hello()
            
          },
          "E": {
            echo 'hola'
            hello()
            
          },
          "C": {
            echo 'hola'
            hello()
            
          }
        )
      }
    }
    stage('sample2') {
      steps {
        echo 'test'
        hello()
      }
    }
  }
}

def hello() {
  
//declarative function
  echo "hello karthik paidi this is declarative with scripted pipeline"
}
