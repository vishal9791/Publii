pipeline {
    agent any

    environment {
        GIT_REPO = 'https://github.com/vishal9791/Publii.git'
        BRANCH = 'main'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/vishal9791/Publii.git'
            }
        }

        stage('Build') {
            steps {
                // Add your build commands here
                echo "Building the project..."
                sh 'echo Build step placeholder'
            }
        }

        stage('Test') {
            steps {
                // Add test commands here
                echo "Running tests..."
                sh 'echo Test step placeholder'
            }
        }

        stage('Deploy') {
            steps {
                // Add deployment commands here
                echo "Deploying the application..."
                sh 'echo Deploy step placeholder'
            }
        }
    }

    post {
        always {
            echo "Cleaning up..."
        }
        success {
            echo "Pipeline succeeded!"
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
