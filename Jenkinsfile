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
                echo 'Building the project...'
                // Your actual build steps would go here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Your actual deploy steps would go here
            }
        }
    }
}
