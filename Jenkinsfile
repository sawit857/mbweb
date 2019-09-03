pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        echo 'checkout code svn'
      }
    }
    stage('Build') {
      steps {
        bat 'bat \'mvn -B -Dmaven.test.skip=true -Dbuild.number=${env.BUILD_ID} clean package\''
      }
    }
  }
}