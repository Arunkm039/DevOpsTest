pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out from Git...'
                git credentialsId: 'git', url: 'https://github.com/Arunkm039/DevOpsTest.git'
            }
        }
        
        stage('Build') {
            steps {
                echo "${env.BRANCH_NAME}"
                // Add your project build steps here. 
                // Assuming a simple Node.js project for example:
                
            }
        }
        
        stage('Deploy') {
            steps {
                echo "${env.BRANCH_NAME}"
                // Here you would add your deployment code.
                // For instance, a script to deploy to your server.
                
                }
            }
        }
    }


