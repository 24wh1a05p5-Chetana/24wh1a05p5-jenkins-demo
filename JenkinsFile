pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Repository cloned successfully'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building Project..."'
                sh 'ls -la'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                mkdir -p deploy
                cp index.html deploy/
                '''
                echo 'Deployment Successful'
            }
        }
    }
}
