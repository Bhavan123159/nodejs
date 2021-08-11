pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/Bhavan123159/nodejs.git'
      }
    }
     
    stage('Build') {
      steps {:
        sh 'npm install'
         sh 'node hello.js'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
