pipeline {
  agent any 
  Stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build'
        archieveArtifacts artifacts: 'dis/trainSchedule.zip'
      }
    }
  }
}
