pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        echo '��GitHub������ĿԴ��'        
      }
    }
    stage('docker-compose') {
      steps {
        echo 'docker-compose'
		docker-compose up -d --build
      }
    }
}