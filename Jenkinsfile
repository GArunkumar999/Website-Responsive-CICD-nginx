pipeline{
    agent any
    stages{
        stage('checkout from scm'){
            steps{
                git branch: 'main', url: 'https://github.com/GArunkumar999/Website-Responsive-CICD-nginx.git'

            }
            
        }
        stage('remove nginx default directory'){
            steps{
                sh 'rm -rf /var/www/html/*'
            }
            
        }
        stage('copy files to html directory'){
            steps{
                sh 'cp -r * /var/www/html/'
            }
        }
    }
    post{
        success{
            echo "BUILD SUCCESS"
        }
        failure{
            echo "BUILD FAILURE"
        }
    }
}
