pipeline {
  agent any
  stages {
    stage("Build"){
      steps {
        echo "First stage"
        sh "./gradlew build --no-daemon"
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
