pipeline {
  agent none
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }

    stage('Static code analysis') {
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