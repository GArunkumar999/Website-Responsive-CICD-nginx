pipeline{
    agent any
    stages{
        stage('checkout from scm'){
            git branch: 'main', url: 'https://github.com/GArunkumar999/Website-Responsive-CICD-nginx.git'
        }
        stage('remove nginx default directory'){
            sh 'rm -rf /var/www/html/*'
        }
    }
}
