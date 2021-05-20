pipeline {
  agent none
  stages {
    stage('Back-End') {
      agent {
        docker {
          image 'maven:3.8.1-adoptopenjdk-11'
        }

      }
      steps {
        sh 'mvn --version'
      }
    }

    stage('Front-End') {
      agent {
        docker {
          image 'node:14-alpine'
        }

      }
      steps {
        sh 'node --version'
      }
    }

  }
}