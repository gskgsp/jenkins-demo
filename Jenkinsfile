pipeline {
	agent any
	
	stages {
		stage('GSK') {
			steps {
				echo 'it is GSK'
			}
		}
		stage('GSK2') {
			steps {
			    git url: 'https://github.com/jenkins-docs/simple-java-maven-app.git'
			    withMaven {
			      sh "mvn clean"
			      sh "mvn install"
			    }
			}
		}
	}
}
