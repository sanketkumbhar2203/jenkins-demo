pipeline {
    agent any

    stages {
        stage('Fetch code') {
            steps {
                git branch: 'main', url: 'https://github.com/sanketkumbhar2203/jenkins-demo.git'
            }
        }
        
        stage('Install Apache') {
            steps {
                sh 'sudo apt install apache2 -y'
            }
        }
        
        stage('Deploy Application') {
            steps {
                sh 'sudo cp -R * /var/www/html/'
            }
        }
    }
}

