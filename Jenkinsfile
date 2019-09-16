pipeline {
  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
   
    stage('Clean') {
      steps {
        sh "mvn clean"
      }
    }
    
    stage('Package') {
      steps {
        sh "mvn package"
      }
    }
  }
}
