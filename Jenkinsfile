pipeline {
	agent { docker 'maven:3.5.0' }
	stages {
		stage('build') {
			steps {
				bat 'mvn --version'
			}
		}
	}
}
