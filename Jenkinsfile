pipeline {
	agent any
	tools {
		maven
	}
	stages {
		stage('Build stage') {
			steps {
				sh 'mvn clean install'
			}
		}	
	}
}