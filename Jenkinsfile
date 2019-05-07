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
        sh 'cd /var/lib/jenkins/workspace/mybatisplus_master/build/libs &'
        sh 'nohup java -jar mybatisplus-0.0.1.jar --spring.profiles.active=int --server.port=8082 &'
      }
    }
  }
}