pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''

./dev/make-distribution.sh --name iganlina-spark --pip --tgz -Dhadoop.version=3.3.1 -DskipTests
'''
      }
    }

  }
}