pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemnon'
        archiveArtifacts artifacts: dist/trainSchedule.zip'
      }
    }
  }
}
