pipeline {
    agent any

    environment {
        BITBUCKET_COMMON_CREDS = credentials('jenkins-bitbucket-common-creds')
    }

    stages {
        stage('Example stage 1') {
            steps {
                echo "BITBUCKET_COMMON_CREDS: ${BITBUCKET_COMMON_CREDS}"
                echo "BITBUCKET_COMMON_CREDS_USR: ${BITBUCKET_COMMON_CREDS_USR}"
                echo "BITBUCKET_COMMON_CREDS_PSW: ${BITBUCKET_COMMON_CREDS_PSW}"
            }
        }
    }
}