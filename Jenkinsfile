pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''export MAVEN_OPTS="-Xss64m -Xmx2g -XX:ReservedCodeCacheSize=1g"

./dev/make-distribution.sh --name iganlina-spark --pip --tgz -Dhadoop.version=3.3.1 -DskipTests
'''
      }
    }

  }
}