pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
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