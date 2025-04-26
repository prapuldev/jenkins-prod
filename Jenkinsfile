pipeline {
    agent any

    stages {
        // stage('Clone Repository') {
        //     steps {
        //         git 'https://github.com/prapuldev/jenkins-prod.git'
        //     }
        // }

        stage('Archive HTML Files') {
            steps {
                sh 'zip -r site.zip .'
            }
        }

        stage('Deploy') {
            steps {
                echo 'In a real scenario, this would copy the files to a web server'
                
            }
        }
    }
}
