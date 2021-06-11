pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/emersonrocha85/nodejs-example-build.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
	    sh 'npm cache clean --force'
        sh 'npm install'
        sh 'npm run bowerInstall'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}