pipeline {
  agent any
  stages {
    stage('Install tools') {
      steps {
        tools(nodejs, "NodeJS14")
      }
    }

    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }

    stage('Build') {
      steps {
        sh 'npm run lint'
        sh 'npm run build'
      }
    }

  }
}