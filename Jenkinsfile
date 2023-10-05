pipeline {
    agent any

    parameters {
		choiceParam {
			name ("ENV")
			description ("Choose target environment")
			choices (['dev', 'qa', 'int'])
		}		

		choiceParam {
			name ("COMPONENT")
			description("Choose component")
			choices (['scheduler', 'worker', 'manager', 'model-worker'])
		}

		choiceParam {
			name ("NAMESPACE")
			description ("Choose namespace")
			choices (['ctad-dev-amp-core', 'ctad-qa-amp-core', 'ctad-int-amp-core'])
		}

	}


    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out from Git...'
                git credentialsId: 'git', url: 'https://github.com/Arunkm039/DevOpsTest.git'
            }
        }
        
        stage('Build') {
            steps {
                echo "${params.ENV}"
                // Add your project build steps here. 
                // Assuming a simple Node.js project for example:
                
            }
        }
        
        stage('Deploy') {
            steps {
                echo "${params.GIT_BRANCH_TAG}"
                // Here you would add your deployment code.
                // For instance, a script to deploy to your server.
                
                }
            }
        }
    }


