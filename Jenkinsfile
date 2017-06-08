pipeline {
  agent any
  stages {
    stage('sample1') {
      steps {
        parallel(
          "A": {
            echo 'some'
            hello()
            post {
              always {
                echo 'Archiving logs and test results...'
                archiveArtifacts '${WORKSPACE}/**'
              }
            }
            
          },
          
          "E": {
            echo 'hola'
            hello()
              post {
                always {
                  echo 'Archiving logs and test results...'
                  archiveArtifacts '${WORKSPACE}/**'
                }
              }
            
          },
          
          "C": {
            echo 'hola'
            hello()
            post {
              always {
                  echo 'Archiving logs and test results...'
                  archiveArtifacts '${WORKSPACE}/**'
              }
            }
            
          }
        )
      }
    }
    
    stage('sample2') {
      steps {
        echo 'test'
        hello()
          post {
            always {
              echo 'Archiving logs and test results...'
              archiveArtifacts '${WORKSPACE}/**'
            }
          }
      }
    }
  }
}

def hello() {
  
//declarative function
  echo "hello karthik paidi this is declarative with scripted pipeline"
}
