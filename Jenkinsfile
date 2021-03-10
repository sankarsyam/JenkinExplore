pipeline {
    agent any
    tools {nodejs "node"}
    stages {
        stage('Verify Branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage('Install dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                bat 'npm test'
            }
        }
         stage('Strt application') {
            steps {
                bat 'npm start'
            }
        }            
    }
}