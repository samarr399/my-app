pipeline {
	agent any

// 	environment {
// 		mavenHome = tool 'jenkins-maven'
// 	}
//
// 	tools {
// 		jdk 'java-17'
// 	}

	stages {

		stage('Install Node'){
			steps {
				sh "apt-get install node"
			}
		}

		stage('Install NPM'){
			steps{
				sh "npm install"
			}
		}

		stage('Build'){
			steps{
				sh "npm build"
			}
		}

		stage('Deploy') {
			steps {
			    sh "npm serve"
			}
		}
	}
}