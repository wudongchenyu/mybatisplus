pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        tool 'Gradle'
        sh 'gradle clean build'
      }
    }
  }
}