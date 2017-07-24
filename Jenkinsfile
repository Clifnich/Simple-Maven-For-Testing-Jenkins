pipeline {
	agent any
	stages {
		stage('build') {
			steps {
				bat "mvn compile | cd C:\'Program Files'\PuTTY | putty.exe -ssh puqian@10.64.207.194 22 -i C:\Users\puqian\keys\private_key.ppk -m C:\Users\puqian\Desktop\script.sh"
			}
		}
	}
}
