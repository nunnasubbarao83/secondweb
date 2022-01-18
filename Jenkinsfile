
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
    
    stage('Maven build')
    {
      steps
      {
     sh 'mvn clean package' 
    }
  } 
   stage('Deploy')
    {
      steps
      {
     sh 'cp /var/lib/jenkins/workspace/Web_app_deploy_on_tomcat/target/SecondWeb.war /usr/share/apache-tomcat/webapps/' 
    }
  }  
  }
}
