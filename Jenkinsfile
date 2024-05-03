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
				bat "xcopy build/* D:/Servers/nginx-1.25.5/html /E /Y"
			}
		}
	}
}