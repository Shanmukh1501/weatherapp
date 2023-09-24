pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                // Get the code from the version control system.
                checkout scm 
            }
        }
        
        stage('Install Dependencies') {
            steps {
                // Install the necessary dependencies.
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Test') {
            steps {
                // Run the test command.
                script {
                    sh 'npm test'
                }
            }
        }
    }
}

