pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '/usr/gradle/gradle-5.4/bin/gradle clean build --debug --scan'
      }
    }
    stage('run') {
      steps {
        sh 'nohup java -jar /build/libs/mybatisplus-0.0.1.jar --spring.profiles.active=int &'
      }
    }
  }
}