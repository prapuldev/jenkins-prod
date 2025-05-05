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
                 echo 'Deploying into to New Server...'
                 sh 'scp -i /var/www/myappnginxserver.pem /var/lib/jenkins/workspace/html-jenkins-pipeline/*.html ubuntu@3.235.169.86:/var/www/html/'
             }
         }
    }
}