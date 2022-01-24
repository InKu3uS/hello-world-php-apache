pipeline {
    agent any
    stage ('build'){
        steps{
            sh 'sudo docker build -t hello-word-php-apache .'
            sh 'sudo docker run -p 80:80 hello-word-php-apache'
        }
            
    }
}

