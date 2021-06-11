pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {
        
       
    stage('Install dependencies') {
      steps {
	    echo 'npm cache clean --force'
        echo 'npm install'
        echo 'npm run bowerInstall'
      }
    }
     
    stage('Test') {
      steps {
         echo 'npm test'
      }
    }      
  }
}