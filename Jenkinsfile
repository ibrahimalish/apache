pipeline {
    agent any

    stages {
        stage('HTML Lint') {
            steps {
                sh 'htmlhint index.html'
            }
        }

        stage('Deploy') {
            steps {
                sh 'sudo cp index.html /var/www/html/index.html'
            }
        }
    }
}
