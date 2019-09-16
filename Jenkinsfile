pipeline {
  agent any
  tools {
    maven 'Maven 3.6'
    jdk 'jdk8'
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
