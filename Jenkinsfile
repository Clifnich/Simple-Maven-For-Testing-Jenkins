pipeline {
	agent any
	stages {
		stage('build') {
			steps {
				bat 'mvn compile | putty.exe -ssh puqian@10.64.207.194 22 -i C:\\Users\\puqian\\keys\\private_key.ppk -m C:\\Users\\puqian\\Desktop\\script.sh'

				echo 'My name is Scary Tom'
			}
		}
		stage('Test Parallel') {
			parallel p1: {
				echo 'Message from P1.'
			}, 
			p2: {
				echo 'Message from P2.'
			}
		}
	}

}
