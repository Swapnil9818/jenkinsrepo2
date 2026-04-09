pipeline {
  agent any
  stages {
    stage('Stage1') {
      agent any
      steps {
        echo '1'
      }
    }

    stage('Stage2') {
      agent any
      steps {
        echo '2'
      }
    }

    stage('Parallel Stages') {
      parallel {
        stage('Parallel Stages') {
          agent any
          steps {
            echo 'parallel'
          }
        }

        stage('Stage3') {
          agent any
          steps {
            echo '3'
          }
        }

        stage('Stage4') {
          agent any
          steps {
            echo '4'
          }
        }

      }
    }

  }
}