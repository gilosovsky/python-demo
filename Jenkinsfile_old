pipeline {
  agent {
    docker {
      image 'python:3.10'  // You can use 3.11 or any other version too
    }
  }
  stages {
    stage('Install') {
      steps {
        sh 'python --version'
        sh 'pip install -r requirements.txt || true'
      }
    }
    stage('Test') {
      steps {
        sh 'python -m unittest test_app.py'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy step placeholder – done!'
      }
    }
  }
}
