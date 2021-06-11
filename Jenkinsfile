pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {
        

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