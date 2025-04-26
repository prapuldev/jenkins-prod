pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning the repository...'
                git branch: 'main', url: 'https://github.com/prapuldev/jenkins-prod.git'
            }
        }

        stage('Build') {
            steps {
                echo 'No build steps needed for HTML project'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to /var/www/html/'
                sh ' cp -r * /var/www/html/'
            }
        }
    }
}
