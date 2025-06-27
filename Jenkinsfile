pipeline {
    agent any
    stages {
        stage('Install') {
            steps {
                sh 'python3 --version'
                sh 'pip3 install -r requirements.txt || true'
            }
        }
        stage('Debug') {
            steps {
             sh 'which python || which python3 || echo "No Python found!"'
             }
        }
        stage('Test') {
            steps {
                sh 'python3 -m unittest test_app.py'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy step placeholder – done!'
            }
        }
    }
}
