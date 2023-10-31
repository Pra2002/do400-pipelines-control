pipeline{
    agent {
        node {
            label 'nodejs'
        }
    } 

    stages{
        stage('checkout'){
            steps{
                git url: 'https://github.com/Pra2002/do400-pipelines-control.git',
                branch: 'main'
            }
        }
        stage('backend'){
            steps{sh 'node ./simple-webapp/backend/test.js'}
            
        }
         stage('frontend'){
            steps{sh 'node ./simple-webapp/frontend/test.js'}
            
        }

    }


}