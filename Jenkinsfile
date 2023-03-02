pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sleep 10
      }
    }

    stage('building the docker image') {
      steps {
        sh 'docker-compose build'
      }
    }

    stage('containerizing') {
      steps {
        sh 'docker-compose up --detach'
      }
    }

  }
}