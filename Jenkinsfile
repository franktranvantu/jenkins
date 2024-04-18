pipeline {
    agent any

    environment { // Apply to all steps within the Pipeline
        CC = 'clang'
    }

    stages {
        stage('Example') {
            environment { // Only apply the given environment variables to steps within the stage.
                DEBUG_FLAGS = '-g'
            }
            steps {
                sh 'printenv'
            }
        }
    }
}