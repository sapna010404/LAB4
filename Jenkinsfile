pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // This stage checks out your source code from the Git repository.
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], userRemoteConfigs: [[url: 'https://github.com/lakshaygogia7/GitTutorial.git']]])
            }
        }
        
        stage('Build') {
            steps {
                // This stage simulates a build step. You should replace this with your actual build commands.
                bat 'echo "Building..."'
            }
        }
        
        stage('Test') {
            steps {
                // This stage simulates a test step. You should replace this with your actual test commands.
                bat 'echo "Testing..."'
            }
        }
    }
    
    post {
        success {
            // This block specifies what to do if the pipeline succeeds.
            echo 'The pipeline has completed successfully.'
        }
        failure {
            // This block specifies what to do if the pipeline fails.
            echo 'The pipeline has failed.'
        }
    }
}
