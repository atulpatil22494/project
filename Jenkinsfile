pipeline {
  agent {
    kubernetes { label 'kubernetes-cloud' }
  }
  
  stages {
    stage('Test') {
      steps {
        sh 'kubectl exec -it -n jenkins jenkins-c8b759cb4-85h5b /bin/bash'
        sh 'cd /var/jenkins_home/workspace/test'
        sh 'kubectl create -f task02.yml'
      }
    }
  }
}
