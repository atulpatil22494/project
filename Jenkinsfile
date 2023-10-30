pipeline {
  agent {kubernetes}
  
  stages {
    stage('Test') {
      steps {
        sh 'kubectl create -f task02.yml'
      }
    }
  }
}
