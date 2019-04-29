pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '/var/jenkins_home/gradle-5.4/bin/gradle clean build --info'
      }
    }
  }
}