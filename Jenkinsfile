pipeline {
  agent {
    kubernetes { label 'kubernetes-cloud' }
  }
  
  stages {
    stage('Test') {
      steps {
        sh 'kubectl create -f task02.yml'
      }
    }
  }
}
