pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'iniciando pipeline...'
        sh 'mvn clean package'
      }
    }
    stage('Test') {
      steps {
        echo 'Iniciando testes...'
        sh 'mvn test'
      }
    }
  }
  environment {
    agent = 'master'
  }
}