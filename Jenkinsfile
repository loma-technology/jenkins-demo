pipeline{
    agent any
    environment{
        staging_server="151.106.120.82"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'scp -r ${WORKSPACE} root@${staging_server}:/var/www/jenkins-demo/'
                   
            }
        }
    }
}
