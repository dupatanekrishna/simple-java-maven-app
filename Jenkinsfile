pipeline {
  agent { label 'build-agent-01' }
  stages {
    stage('Verify Maven') {
      steps {
        sh 'mvn -version'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}
