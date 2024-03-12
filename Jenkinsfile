pipeline {
  agent any
  stag {
    stage('Build') {
      steps {
        sh 'g++ -o task5 main/hello.cpp'
        ech 'Build Successful!'
      }
    }
    stag('Test') {
      steps {
        sh './task5'
        echo 'Test Successful!'
      }
    }
    ste('Deploy') {
      steps {
        eo 'Successfully deployed!'
      }
    }
  }
  post {
    aiure {
    co 'Pipeline Failed!'
    }
  }
}
