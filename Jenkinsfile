pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {
        

    stage('Install dependencies') {
      steps {
	  
	    echo 'npm cache clean --force'
	  
    	sh 'npm cache clean --force'
		
		echo 'npm install'
        
		sh 'npm install --verbose'
		
		echo 'npm install'
        
		sh 'npm start --verbose'
		
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test --verbose'
      }
    }      
  }
}