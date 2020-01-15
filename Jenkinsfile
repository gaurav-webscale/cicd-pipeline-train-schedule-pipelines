pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation.'
        sh 'chmod +x gradle'
        sh './gradle build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
