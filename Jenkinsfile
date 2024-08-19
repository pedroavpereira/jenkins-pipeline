// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// 	stage('Integration Test'){
// 		echo "Integration Test"
// 	}
// }


// node{
// 	echo "Build"
// 	echo "Test"
// 	echo "Integration Test"
// }

pipeline{
	agent any
	// agent{
	// 	docker{
	// 		image "maven:3.9.8"
	// 	}
	// }
	stages{
		stage("Build"){
			steps{
				// sh "mvn --version"
				echo "Build"
				echo "Path: $PATH"
				echo "Build Number: $env.BUILD_NUMBER"
				echo "Build ID: $env.BUILD_ID"
				echo "Build Tag: $env.BUILD_TAG"
				echo "Build URL: $env.Build_URL"
				echo "JOB NAME: $env.JOB_NAME"
			}
			post{
				always{
					echo "I run at the end of the building stage"
				}
			}
		}
		stage("Test"){
			steps{
				echo "Test"
			}
		}
		stage("Integration Test"){
			steps{
				echo "Integration Test"

			}
		}
	}
	post{
		always{
			echo "I always run"
		}
		success{
			echo "I run when successfull"
		}
		failure{
			echo "I run when failed"
		}
	}
}


