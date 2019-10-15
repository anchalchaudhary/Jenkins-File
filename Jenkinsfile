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
        maven 'M2'
      }
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
