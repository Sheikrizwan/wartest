pipeline {
	agent any
	stages {
		stage('Build stage') {
			steps {
				sh 'mvn clean install'
			}
		}
		stage('Docker Image build') {
			steps {
				sh 'docker build . -t sheikrizwan/warfile:v1'
			}
		}	
	}
}
