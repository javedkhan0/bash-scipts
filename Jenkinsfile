pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/javedkhan0/HelloWorld-Springboot-App.git', branch: 'master')
      }
    }

    stage('test') {
      steps {
        sh 'sh \'mvn clean\''
      }
    }

    stage('build') {
      steps {
        sh 'sh \'mvn package\''
      }
    }

  }
}