pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '/usr/gradle/gradle-5.4/bin/gradle clean build --debug --scan'
      }
    }
  }
}