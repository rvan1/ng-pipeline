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
                sh 'npm install -g karma && npm install -g karma-cli'
                sh 'karma start'
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy'
            }
        }
    }
}
