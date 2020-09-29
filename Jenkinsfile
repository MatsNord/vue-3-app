pipeline {
  agent any

  tools(nodejs, "NodeJS14")
  stages {  
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