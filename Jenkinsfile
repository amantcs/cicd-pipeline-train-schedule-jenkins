pipeline{
  agent ("linux-node")
  stages{
    stage ('Build') {
      steps {
        echo 'Running build Automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
