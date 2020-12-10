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
			    git url: 'https://github.com/cyrille-leclerc/multi-module-maven-project'
			    withMaven {
			      sh "mvn clean"
			      sh "mvn install"
			    }
			}
		}
	}
}
