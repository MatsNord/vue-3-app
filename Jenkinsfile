pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }

    stage('static coda analysis') {
      steps {
        sh 'npm run lint'
      }
    }

    stage('build') {
      steps {
        sh 'npm run build'
      }
    }

  }
}