pipeline {
  
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
        script {
          sh 'kubectl apply -f deployment.yaml -f service.yaml -f ingress.yaml'
        }
      }
    }
  }
}
