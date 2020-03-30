pipeline {
  agent any
  stages {
    stage('SCA') {
      agent {
        node {
          label 'master'
        }

      }
      steps {
        echo 'SCA'
      }
    }

    stage('Build') {
      agent {
        node {
          label 'AEM'
        }

      }
      steps {
        echo 'Hello'
        sh 'ifconfig'
      }
    }

    stage('Deploy') {
      agent {
        node {
          label 'master'
        }

      }
      steps {
        echo 'Deploy to JBoss'
      }
    }

  }
}