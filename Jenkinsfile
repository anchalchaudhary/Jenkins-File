pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/anchalchaudhary/time-tracker.git'
      }
    }
    stage('Compile') {
      tools {
        maven 'Maven'
      }
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
