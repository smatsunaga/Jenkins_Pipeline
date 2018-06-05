pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('hello world') {
      steps {
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
    TEST_USER = credentials('test-user')
  }
}