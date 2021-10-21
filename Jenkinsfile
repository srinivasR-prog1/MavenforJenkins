pipeline{
    agent any
	stages{	
	   stage('Compile Stage'){
	   
	     steps{
		 
		    bat 'mvn clean compile'		 
		 
		 
		 }
	   
	   
	   
	   }
	   
	   stage('Testing Stage'){
	   
	     steps{
		 
		    bat 'mvn test'		 
		 
		 
		 }
	   
	   
	   
	   }
	   
	   stage('Install Stage'){
	   
	     steps{
		 
		    bat 'mvn install'		 
		 
		 
		 }
	   
	   
	   
	   }
	
	
	
	}

     post
	{
	
	  always
		{
		
		  emailext body: 'Summary', subject: 'Pipeline status', to: 'sri1.as400@gmail.com'
		
		
		}
	
	
	
	}


}
