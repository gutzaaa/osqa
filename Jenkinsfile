pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build16') {
          steps {
            sh 'echo \'ok\';'
          }
        }
        stage('build2') {
          steps {
            echo 'ok'
          }
        }
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'ok lah'
          }
        }
        stage('test@2') {
          steps {
            echo '222'
          }
        }
      }
    }
    stage('jii') {
      steps {
        echo 'ok'
      }
    }
  }
}