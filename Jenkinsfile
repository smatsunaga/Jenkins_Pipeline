pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('hello world') {
      steps {
        sh 'java -version'
        echo "Hello ${MY_NAME} and ${params.Name}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are & me', description: 'Who should I say hi to?')
  }
}