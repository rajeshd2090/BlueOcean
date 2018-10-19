pipeline {
  agent any
  stages {
    stage('Clone Code') {
      steps {
        git 'https://github.com/rajeshd2090/Secure-tomcat-docker.git'
      }
    }
    stage('Transfer Code') {
      steps {
        sshPublisher(masterNodeName: 'k8-host')
      }
    }
  }
}