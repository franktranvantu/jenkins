pipeline {
    agent any

    environment {
        EXAMPLE_CREDS = credentials('example-credentials-id')
    }

    stages {
        stage('Example') {
            steps {
                echo "${EXAMPLE_CREDS_USR}"
            }
        }
    }
}