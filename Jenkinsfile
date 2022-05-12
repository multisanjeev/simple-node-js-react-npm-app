pipeline {
	agent any
	
	stages {
		stage('build') {
			steps {
				sh 'sudo npm install'
				sh 'sudo npm run build'
			}
		}
		stage('Deploy') {
			steps {
				sh "sudo rm -rf /var/www/html/jenkins-react-app"
				sh "sudo cp -r ${WORKSPACE}/build/ /var/www/html/jenkins-react-app/"
			}
		}
	}
}
