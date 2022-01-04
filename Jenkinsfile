pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''export MAVEN_OPTS="-Xss4096m -Xmx28g -XX:ReservedCodeCacheSize=3g"

./dev/make-distribution.sh --name iganlina-spark --pip --tgz -Dhadoop.version=3.3.1 -DskipTests
'''
      }
    }

  }
}