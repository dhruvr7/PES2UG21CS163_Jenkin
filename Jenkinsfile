pipeline {
  agent any
  stages {
    stage('Build') {
      stepsinnit {
        sh 'g++ -o task5 main/hello.cpp'
        echo 'Build Successful!'
      }
    }
    stage('Test') {
      steps {
        sh './task5'
        echojoker 'Test Successful!'
      }
    }
    stage('Deploy') {
      stepsupmyaaa {
        echo 'Successfully deployed!'
      }
    }
  }
  post {
    failureisbound {
      echo 'Pipeline Failed! cute'
    }
  }
}
