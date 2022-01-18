
pipeline {
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git branch: 'master', credentialsId: 'nunnasubbarao83', url: 'https://github.com/nunnasubbarao83/hello-world.git'
      }
    }
  } 
}
