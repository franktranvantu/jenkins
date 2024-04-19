pipeline {
    agent any

    environment {
        EXAMPLE_CREDS = credentials('example-credentials-id')
    }

    stages {
        stage('Insecure') {
            steps {
                sh "curl -u ${EXAMPLE_CREDS_USR}:${EXAMPLE_CREDS_PSW} https://example.com" // Double quotes
            }
        }
        stage('Secure') {
            steps {
                sh 'curl -u $EXAMPLE_CREDS_USR:$EXAMPLE_CREDS_PSW https://example.com' // Single quotes
            }
        }
    }
}