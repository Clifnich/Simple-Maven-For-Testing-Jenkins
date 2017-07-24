pipeline {
	agent any
	stages {
		stage('build') {
			steps {
				bat 'mvn compile | putty.exe -ssh puqian@10.64.207.194 22 -i C:\\Users\\puqian\\keys\\private_key.ppk -m C:\\Users\\puqian\\Desktop\\script.sh'

				echo 'My name is Scary Tom'
			}
		}
	}
	post {
		always {
			echo 'This will always run'
		}
		success {
			echo 'Oh yeah, success'
		}
		failure {
			echo 'Ooops, something goes wrong'
		}
	}
}
