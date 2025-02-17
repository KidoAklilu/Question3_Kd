pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/KidoAklilu/simple-repo.git'
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
