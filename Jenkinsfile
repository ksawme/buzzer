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
        stage('') {
          steps {
            sh '''file=README.md
if [ ! -e "$file" ]; then
    echo "File does not exist"
else 
    echo "File exists"
fi '''
          }
        }
      }
    }
  }
}