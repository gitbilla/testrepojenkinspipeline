pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Building'
      }
    }

    stage('Backend') {
      parallel {
        stage('Unit') {
          steps {
            sh 'echo Unit'
          }
        }

        stage('Performance') {
          steps {
            sh 'echo performance'
          }
        }

      }
    }

    stage('Frontend') {
      steps {
        sh 'echo Frontend'
      }
    }

    stage('Analysis') {
      steps {
        sh 'echo analysis'
      }
    }

    stage('deploy') {
      steps {
        sh 'echo deploy'
      }
    }

  }
}
