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
    }
}
