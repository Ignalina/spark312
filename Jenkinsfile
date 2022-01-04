pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''export MAVEN_OPTS="-Xss1024m -Xmx8g -XX:ReservedCodeCacheSize=2g"

./dev/make-distribution.sh --name iganlina-spark --pip --tgz -Dhadoop.version=3.3.1 -DskipTests
'''
      }
    }

  }
}