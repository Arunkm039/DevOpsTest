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
                echo 'Building...'
                // Add your project build steps here. 
                // Assuming a simple Node.js project for example:
                
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Here you would add your deployment code.
                // For instance, a script to deploy to your server.
                
                }
            }
        }
    }
    
    post {
        failure {
            echo 'Deployment failed...'
        }
        success {
            echo 'Deployment completed successfully!'
        }
    }
}
