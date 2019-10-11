pipeline {
  agent any
  stages {
    stage('S1') {
      parallel {
        stage('S1') {
          steps {
            sh 'echo "This is STEP 1"'
          }
        }
        stage('S12') {
          steps {
            sh 'echo "This is PARALLEL Step"'
          }
        }
      }
    }
    stage('S2') {
      steps {
        sh 'echo "This is STEP2"'
      }
    }
    stage('S3') {
      steps {
        sh 'echo "Final STEP"'
      }
    }
  }
}