pipeline {
	agent any
	
	stages {
		stage('build') {
			steps {
				sh 'sudo npm install'
				sh 'sudo npm run build'
			}
		}
	}
}
