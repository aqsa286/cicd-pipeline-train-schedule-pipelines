pipeline {
  agent any 
  Stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        ./gradlew build --no-daemon
        archieveArtifacts artifacts: 'dis/trainSchedule.zip'
      }
    }
  }
}
