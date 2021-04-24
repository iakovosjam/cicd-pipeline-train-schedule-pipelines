pipeline {
  agent any
  stages {
    stage("build") {
      echo 'Running build automation.'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
