pipeline {
  agent {
    kubernetes { label 'jenkins' }
  }
  
  stages {
    stage('Test') {
      steps {
        sh 'kubectl create -f task02.yml'
      }
    }
  }
}
