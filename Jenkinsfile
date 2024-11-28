pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build commands here
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment commands here
            }
        }
    }

    post {
        always {
            echo 'This runs regardless of build success or failure.'
        }
        success {
            echo 'Build succeeded!'
            // Add actions to perform on a successful build, such as notifications
        }
        failure {
            echo 'Build failed!'
            // Add actions to perform on a failed build, such as error reporting
        }
        unstable {
            echo 'Build is unstable!'
            // Add actions for unstable builds if necessary
        }
        aborted {
            echo 'Build was aborted!'
            // Add actions for aborted builds
        }
    }
}
