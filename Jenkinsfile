pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'Hello world'
            git(url: 'https://github.com/Kumarobin/known-Blueocean.git', branch: 'main')
          }
        }

        stage('stage3') {
          steps {
            sleep 300
          }
        }

      }
    }

    stage('stage2') {
      steps {
        sh 'whoami'
      }
    }

    stage('stage3') {
      steps {
        echo 'Hello'
      }
    }

  }
}