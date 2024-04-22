pipeline{
	agent {
		docker {
			image 'maven:3.6.3'
		}
	}
	stages{
		stage('Build'){
			steps{
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage('test'){
			steps{
				echo "test"
			}
		}
		stage('Integration test'){
			steps{
				echo "Integration test"
			}
		}
	
	}
	
	post{
		always{
			echo "i always run"
		}
		success{
			echo "i run on success"
		}
		failure{
			echo "i run on failure"
		}
		changed{
			echo "i run if status chages for pipeline run"
		}
	}


}