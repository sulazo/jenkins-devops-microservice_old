pipeline{
	//agent{docker{image 'maven:3.6.3}}  ---means you want to build inside a Maven image,jenkins will pull image and run the build inside it
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
