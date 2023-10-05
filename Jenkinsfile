pipeline {
    agent any

     parameters {
                choiceParam('ENV', ['dev', 'qa', 'int'], 'Description for choice parameter')
                gitParameter(name: 'GIT_BRANCH_TAG', type: 'PT_BRANCH', branch: '*', defaultValue: '""', description: 'Git Parameter')  // Assuming you have Git Parameter plugin
                booleanParam('RUN_TESTS', true, 'unit test')
                booleanParam('SONAR_SCAN', false, 'sonar scan')
            }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out from Git...'
                git credentialsId: 'Github', url: 'https://github.com/Arunkm039/DevOpsTest.git'
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
