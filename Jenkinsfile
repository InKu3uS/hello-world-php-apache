pipeline {
    agent any
    stages {
        stage ('Build'){
            steps{
                sh 'docker build -t hello-world-php-apache .'
                sh 'docker run -d --rm -p 8085:80 hello-world-php-apache'
            }
        }
        stage('Test'){
            steps{
                sh 'wget http://localhost:8085/'
            }
        }
    }
}

