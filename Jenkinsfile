pipeline {
	agent any
	
	tools {
		gradle 'Gradle'
		jdk 'JDK'
	}
	
	stages {
		stage('Checkout') {
			steps {
				git branch: 'main', url: 'https://github.com/gkongit/MyGradleApp.git'
			}
		}
		
		stage('Build') {
			steps {
				sh 'gradle build'
			}
		}
		
		stage('Run') {
			steps {
				sh 'gradle run'
			}
		}
		
		stage('Display') {
			steps {
				sh 'gradle display'
			}
		}
	}	
}
