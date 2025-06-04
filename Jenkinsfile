pipeline {
	agent any
	
	tools {
		gradle 'Gradle'
		jdk 'JDK'
	}
	
	stages {
		stage('Checkout') {
			git branch: 'main', url: ''
		}
		
		stage('Build') {
			sh 'gradle build'
		}
		
		stage('Run') {
			sh 'gradle run'
		}
		
		stage('Display') {
			sh 'gradle display'
		}
	}	
}
