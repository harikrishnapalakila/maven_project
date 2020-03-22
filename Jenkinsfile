pipeline{
	agent any
	
	environment {
		PATH = "${PATH}:D:/Krishna/Binaries/apache-maven-3.6.0-bin/apache-maven-3.6.0/bin"
	}
	stages{
	
		stage('SCM - Checkout'){
			steps{
				git url: 'https://github.com/javahometech/myweb'
			
			}
		}
	
	
	 	stage('Maven Build - Clean - Test'){
			steps{
			bat "mvn clean"
			
			}
 	}
	
		
		
		
		
	}
 }
