pipeline {
    agent any

    parameters {
        choice(name: 'DEPLOY_ENV', choices: ['Development', 'Staging', 'Production'], description: 'Select environment to deploy to')
        string(name: 'GIT_BRANCH_TAG', defaultValue: 'master', description: 'Git branch or tag for deployment')
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
                echo "${params.DEPLOY_ENV}"
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
