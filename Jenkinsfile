pipeline{
    agent any
    stages {
        stage ('setup'){
            steps{
                cleanWs();
            sh 'echo setting up my workspace'
            }
stage ('checkoyt scm'){
    steps{
        checkout scm
    }
    stage ('compile Code'){
        steps {
            sh 'chmod +x app.sh'
        }
        stage ('Testing'){
            steps{
                sh 'sh app.sh'
            }
            stage ('deploy'){
            steps{
                sh 'echo deploy'
            }
        }
    }
}
            
        }
    }
}