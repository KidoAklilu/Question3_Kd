pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git credentialsId: 'a3579465-0d06-4b16-b5a7-8f45c439dd9c', branch: 'main', url: 'https://github.com/KidoAklilu/Question3_Kd.git'
            }
        }
        stage('Build') {
            steps {
                echo "JENKINS_URL: ${env.JENKINS_URL}"
                echo "BUILD_ID: ${env.BUILD_ID}"
            }
        }
    }
    triggers {
        githubPush()
    }
}
