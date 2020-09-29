pipeline {
  agent any
  stages {
    stage('Install tools') {
      steps {
        tool(name: 'NodeJS14', type: 'nodejs')
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