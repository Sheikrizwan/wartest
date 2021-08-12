pipeline {
	agent any
	tools {
		maven 'apache-maven-3.8.1'
	}
	stages {
		stage('Build stage') {
			steps {
				sh 'mvn clean install'
			}
		}	
	}
}
