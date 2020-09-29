pipeline {
  agent any

 nodejs('NodeJS14') {
  stages {

    stage('Install') {
      steps {
        sh 'npm config ls'
        sh 'which node'
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
}