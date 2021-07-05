pipeline {
    agent any
  stages {
    stage('Test Alpine') {
      steps {
        container('alpine') {
          sh """
            echo Alpine
          """
        }
      }
    }
    stage('Test Alpine2') {
      steps {
        container('alpine2') {
          sh "echo Alpine2"
        }
      }
    }
    stage('Test Alpine3') {
      steps {
        container('alpine3') {
          sh("echo Alpine3")
        }
      }
    }
  }
}
