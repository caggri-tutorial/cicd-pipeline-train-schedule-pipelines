pipeline {
  agent any
  stages {
    stage("Build"){
      steps {
        echo "First stage"
        bash "./gradlew build --no-daemon"
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
