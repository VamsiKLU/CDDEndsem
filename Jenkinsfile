pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                checkout scm
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploying file..."
                cp index.html /var/www/html/index.html
                '''
            }
        }
    }
}
