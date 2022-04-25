pipeline{
    agent any
    stages{

        stage('Continuous Download'){
			steps{
            echo "Download"


			}
        }
        stage('Continuous Build'){
			steps{
            echo "Build"

			}

        }
        stage('Continuous Deploy'){
			steps{

            echo "Deploy"

			}

        }
        stage('Continuous Delivery'){
			steps{
            echo "Delivery"

			}

        }
    }
post{
	always{
		echo "I run always"
	}
	success{

    echo "i run when successful"
	}
	failure{
	echo "failed"
	}
}


}
