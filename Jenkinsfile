
pipeline{
    agent any;
    stages{
        stage('setup'){
            steps{
                cleanWs()
                sh 'echo settingup my workspace'
            }
        }
            stage('checkoutscm'){
            steps{
                checkout scm
            }
        }
        stage('compile'){
            steps{
                sh 'chmod +x app.sh'
            }
        }
        stage('testing'){
            steps{
                sh  'app.sh'
            }
        }
    }
}
