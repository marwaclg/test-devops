pipeline {
  agent {
    node {
      label 'node1'
    }

  }
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh 'grep user /etc/passwd'
          }
        }

        stage('stage2') {
          steps {
            sh 'ls /var/lib/jenkins'
          }
        }

      }
    }

    stage('error') {
      steps {
        sh 'ifconfig'
      }
    }

  }
}