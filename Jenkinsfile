pipeline {
    agent any

    environment {
        EXAMPLE_CREDS = credentials('example-credentials-id')
    }

    stages {
        stage('Secure') {
            steps {
                echo '$EXAMPLE_CREDS_USR'
                echo '$EXAMPLE_CREDS_PSW'
            }
        }
    }
}