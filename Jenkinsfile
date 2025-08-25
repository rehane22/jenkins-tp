pipeline {
  agent any
  tools { nodejs 'Node20' } 
  
  stages {
    stage('Checkout') {
      steps { checkout scm }
    }
    stage('Install') {
      steps { sh 'npm ci || npm install' }
    }
    stage('Build') {
      steps { sh 'npm run build' }
    }
    stage('Test') {
      steps { sh 'npm test' }
    }
  }
 /*  vebje */
}
