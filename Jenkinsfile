pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is dev stage'
      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            echo 'this is staging area'
          }
        }

        stage('stage1') {
          steps {
            echo 'this is staging 1 area'
          }
        }

      }
    }

    stage('step') {
      parallel {
        stage('step') {
          steps {
            echo 'this is steps area'
          }
        }

        stage('access') {
          steps {
            echo 'his is access area'
          }
        }

      }
    }

    stage('echo') {
      steps {
        echo 'this is echo area'
      }
    }

    stage('end ') {
      steps {
        echo 'this is the end of the pipeline'
      }
    }

  }
}