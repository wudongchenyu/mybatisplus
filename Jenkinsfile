pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '${tool \'Gradle\'}/bin/gradle clean build'
      }
    }
  }
}