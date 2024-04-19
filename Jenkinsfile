pipeline {
    agent any

    environment {
        MY_KUBECONFIG = credentials('my-kubeconfig')
    }

    stages {
        stage('Example stage 1') {
            steps {
                sh "kubectl --kubeconfig $MY_KUBECONFIG get pods"
            }
        }
    }
}