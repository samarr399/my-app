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

		stage('Build'){
			steps {
				sh "apt-get install node"
			}
		}

		stage('Install'){
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