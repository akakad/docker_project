pipeline {
  agent {
    docker {
      image 'ubuntu:latest'
    }
  }
  stages {
    stage('Build') {
      steps {
        sh 'apt-get upadte -y'
      }
    }
    stage('Deploye') {
      steps {
        sh 'apt-get install docker.io -y' 
      }
    }
    stage('test') {
      steps {
        sh 'sudo docker systemctl docker start'
        sh 'docker -vesrion'
      }
    }
  }
}
