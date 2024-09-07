pipeline {
  agent none

  stages {

    stage('maven') {
      agent { docker "maven" }
      steps {
        sh "mvn -version"
        sh "java -version"
      }
    }

    stage('node') {
      agent { docker "node" }
      steps {
        sh "node --version"
      }
    }

    stage('python') {
      agent { docker "python" }
      steps {
        sh "python3 --version"
      }
    }

    stage('golang') {
      agent { docker "golang" }
      steps {
        sh "go version"
      }
    }

    stage('gradle') {
      agent { docker "gradle" }
      steps {
        sh "gradle --version"
      }
    }

  }
}

