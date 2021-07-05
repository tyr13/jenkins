pipeline {
    agent { any }
/*  agent {
    kubernetes {
      yaml """
apiVersion: v1
kind: Pod
metadata:
labels:
  component: ci
spec:
  # Use service account that can deploy to all namespaces
  serviceAccountName: jenkins
  containers:
  - name: alpine
    image: alpine:latest
    command:
    - cat
    tty: true
  - name: alpine2
    image: alpine:latest
    command:
    - cat
    tty: true
  - name: alpine3
    image: alpine:latest
    command:
    - cat
    tty: true
"""
}
  } */
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
