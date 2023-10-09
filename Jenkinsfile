pipeline {
    agent any

     triggers {
        pollSCM('H/2 * * * *')  // polls every 5 minutes, adjust as needed
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the current branch
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "${env.BRANCH_NAME}"
                // Your actual build steps would go here
            }
        }

        stage('Deploy') {
            steps {
                echo "${env.BRANCH_NAME}"
                // Your actual deploy steps would go here
            }
        }
    }
}
