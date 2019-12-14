pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        echo '从GitHub下载项目源码'
      }
    }
	stage('workspace') {
      steps {
		echo 'cd /var/jenkins_home/workspace/Mainpipeline'
        cd /var/jenkins_home/workspace/WorkflowPipeline
      }
    }
    stage('docker-compose') {
      steps {
        echo 'docker-compose'
		echo 'docker-compose up --build'
      }
    }
}