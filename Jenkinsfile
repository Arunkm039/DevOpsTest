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

            }
        }

        stage('Deploy') {
            steps {
                echo "${env.BRANCH_NAME}"

            }
        }
    }
}
