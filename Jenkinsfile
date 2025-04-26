pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/prapuldev/jenkins-prod.git'
            }
        }

        stage('Build') {
            steps {
                echo 'No build steps needed for HTML project'
            }
        }

        stage('Deploy to New Server') {
            steps {
                echo 'Deploying to New Server...'
                sh 'scp -o StrictHostKeyChecking=no -i /var/www/mywebserver.pem /var/www/html/* ubuntu@56.228.14.159:/var/www/html/'
            }
        }
    }
}
