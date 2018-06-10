pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'npm start'
          }
        }
        stage('error') {
          steps {
            sh '[ -f README.md ] && echo "File exist" || echo "File does not exist"'
          }
        }
      }
    }
  }
}