pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/javedkhan0/HelloWorld-Springboot-App.git', branch: 'master')
      }
    }

    stage('compile') {
      steps {
        sh 'mvn clean install'
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean package'
      }
    }

  }
}
