pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps { 
                echo 'build'
                sh 'npm install'
            }
        }
        stage('Test'){
            steps {
                echo 'test'
                sh 'npm install -g karma-cli'
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy'
            }
        }
    }
}
