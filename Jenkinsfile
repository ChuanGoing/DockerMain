pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        echo '从GitHub下载项目源码'        
      }
    }
    stage('docker-compose') {
      steps {
        echo 'docker-compose'
		docker-compose up -d --build
      }
    }
}