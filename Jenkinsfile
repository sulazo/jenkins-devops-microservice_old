pipeline{
	//agent{docker{image 'maven:3.6.3}}  ---means you want to build inside a Maven image,jenkins will pull image and run the build inside it
	//u can use node:13.8 etc
    agent any
	environment {
		// dockerHome = tool 'myDocker'
		mavenHome  = tool 'myMaven'
		PATH ="$mavenHome/bin:$PATH"
		// PATH ="$dockerHome/bin:$mavenHome/bin:$PATH"
	}
    stages{

        stage('Continuous Download'){
			steps{
				sh 'mvn --version'
				sh "docker version"
              echo "Download"
			  echo "PATH -$PATH"
			  echo "BUILD_NUMBER - $env.BUILD_NUMBER"
			  echo "BUILD_ID - $env.BUILD_ID"
			  echo "JOB_NAME - $env.JOB_NAME"
			  echo "BUILD_TAG - $env.BUILD_TAG"
			  echo "BUILD-URL -$env.BUILD_URL"

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
