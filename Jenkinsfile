pipeline{
	agent any
	
	environment {
		PATH = "${PATH}:D:/Krishna/Binaries/apache-maven-3.6.0-bin/apache-maven-3.6.0/bin"
	}
	stages{
	
		stage('SCM - Checkout'){
			steps{
			git credentialsId: 'git_Credentials', url: 'https://github.com/harikrishna12334/maven_project.git'
			
			}
		}
	
	
	    stage('maven'){
			stage('Maven Build'){
					steps{
					bat "mvn clean test"
			}
 	}
	}
  }
}
