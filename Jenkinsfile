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
	
	
	 	stage('Maven Build - Clean'){
			steps{
			bat "mvn clean"
			
			}
 	}
	
		
		stage('Maven Build - Test'){
			steps{
			bat "mvn test"
			
			}
 	}
	
		stage('Maven Build - PKG with Rename war file'){
			steps{
			bat "mvn package"
			bat "rename target\\myweb-8.3.2.war myweb.war"
			
			}
 	}
		
		
		
	}
 }
