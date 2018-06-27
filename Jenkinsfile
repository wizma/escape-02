pipeline {
  agent any
  stages {
    stage('First stage') {
      agent {
        node {
          label 'local'
        }

      }
      steps {
        echo 'The first message'
        echo 'after the first message'
      }
    }
    stage('Second Stage') {
      agent {
        node {
          label 'master'
        }

      }
      steps {
        echo 'The second message'
      }
    }
  }
}