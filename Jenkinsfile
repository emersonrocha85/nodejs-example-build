pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {

    stage('NPM Cache Clean') {
      steps {
	  
	    echo 'npm cache clean --force'
	  
    	sh 'npm cache clean --force'
	
      }
    }        

    stage('NPM Install') {
      steps {
	  
		echo 'npm install'
        
		sh 'npm install --verbose'

      }
    }

    stage('Build') {
      steps {

		echo 'npm run build'
        
		sh 'npm run build --verbose'
		
      }
    }
     
    stage('Test') {
      steps {
         echo 'npm test --verbose'
      }
    }      
  }
}