pipeline {
	agent any

	stages {
		stage('Install NPM'){
			steps{
				bat "npm install"
			}
		}

		stage('Build'){
			steps{
				bat "npm run build"
			}
		}

		stage('Deploy') {
			steps {
				bat "npx serve -s build"
			}
		}
	}
}