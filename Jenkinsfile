pipeline {
  agent any

  stages {
    stage('Clean UP') {
      steps {
        cleanWs()
      }
    }
    stage('Code Check out') {
      steps {
        git branch: 'master',
            url: 'https://github.com/wasiqali22/full-stack_chatApp.git'
      }
    }
    stage('Deploy') {
      steps {
        script {
          sh 'docker compose up -d --build'
        }
      }
    }
  }
}
