pipeline {
    agent {
        docker {
            image 'node:16'
        }
    }
    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building the project...'
                    sh 'npm install --save'
                }
            }
        }
    }
    post {
        success {
            echo 'Build successfull!'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
