pipeline {
    agent any

     
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
