
pipeline{
  
  agent any
  
  stages {
    
    stage('checkout codebase'){
      steps{
            cleanWs()
        checkout scm: [class: 'GitSCM', branches: [[name: '*/main']],userRemoteConfigs: [[credentialsId: 'github-ssh-key', url: 'git@github.com:ibrahimhanna/demo1.git']]
      }
      
    }
    
                       stage('build'){
                         
                         steps{
                           sh 'mkdir lib'
                           
                         }
                       }
                       
    
  }
  
  
  
}
