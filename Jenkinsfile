pipeline {
  agent any
  tools {
    maven 'Maven 3.6'
    jdk 'JDK1.8'
  }
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
