pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        tool 'Gradle'
        sh '/var/jenkins_home/gradle-5.4/bin/gradle clean build'
      }
    }
  }
}
