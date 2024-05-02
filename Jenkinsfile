pipeline {
	agent any

	stages {
		stage('Install NPM'){
			steps{
				sh "npm install"
			}
		}

		stage('Build'){
			steps{
				sh "npm run build"
			}
		}

		stage('Deploy') {
			steps {
				sh "npm install -g serve"
			    sh "serve -s build"
			}
		}
	}
}