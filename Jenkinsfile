pipeline {
	agent any
	stages {
		stage('build') {
			steps {
				

				echo 'My name is Scary Tom'
			}
		}
		stage('Test Parallel') {
			steps {
				parallel p1: {
					bat 'mvn compile | putty.exe -ssh puqian@10.64.207.194 22 -i C:\\Users\\puqian\\keys\\private_key.ppk -m C:\\Users\\puqian\\Desktop\\script.sh'
				}, 
				p2: {
					bat 'mvn compile | putty.exe -ssh puqian@10.64.207.181 22 -i C:\\Users\\puqian\\keys\\private_key.ppk -m C:\\Users\\puqian\\Desktop\\script.sh'
				}
			}
			
		}
	}

}
