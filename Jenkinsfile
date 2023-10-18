pipeline {
  agent {
    node {
      label 'node1'
    }

  }
  stages {
    stage('stage1') {
      steps {
        sh 'grep user /etc/passwd'
      }
    }

    stage('') {
      steps {
        sh 'ifconfig'
      }
    }

  }
}