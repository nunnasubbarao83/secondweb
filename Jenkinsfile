
pipeline {
  
   tools { 
        maven 'maven' 
        jdk 'java' 
    }
  
  agent any
  
  stages {
    stage('Cloning Git') {
      steps {
        git branch: 'master', credentialsId: 'nunnasubbarao83', url: 'https://github.com/nunnasubbarao83/secondweb.git'
      }
    }
    
    stage('build')
    {
      steps
      {
     sh 'mvn clean package' 
    }
  } 
}
