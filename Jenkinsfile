pipeline{
	//agent any
	agent { docker { image 'maven:3.9.7'} }
	stages{
		stage('Build'){
			steps{
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}
	post{
		always{
			echo "Iam awesome. I run always"
		}
		success{
			echo " success"
		}
		failure{
			echo "failure"
		}
	}
}