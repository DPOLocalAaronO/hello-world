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
      def workspace = pwd()
      steps {
        echo 'Deploying....'
        sh 'echo ${workspace}'
      }
    }
  }
}
