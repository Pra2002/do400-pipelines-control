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
            sh 'node ./simple-webapp/backend/test.js'
        }
         stage('frontend'){
            sh 'node ./simple-webapp/frontend/test.js'
        }

    }


}