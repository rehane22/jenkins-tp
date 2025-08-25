pipeline {
  agent any

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

 /*  post {
    success { echo '✅ Pipeline terminé avec succès' }
    failure { echo '❌ Pipeline échoué' }
    always  { echo '🏁 Fin de l’exécution' }
  } */
}
