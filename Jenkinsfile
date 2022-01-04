pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''export MAVEN_OPTS="-Xss256m -Xmx25g -XX:ReservedCodeCacheSize=2g"

./dev/make-distribution.sh --name iganlina-spark --pip --tgz -Dhadoop.version=3.3.1 -DskipTests
'''
      }
    }

  }
}