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
		stage('deploy') {
			steps {
				deploy adapters: [tomcat8(credentialsId: 'Tomcat_credentials', path: '', url: 'http://3.144.47.200:8080/')], contextPath: null, war: '**/*.war'
			}
		}	
	}
}
