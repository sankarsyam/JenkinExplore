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
                sh 'npm install'
            }
            }
            
            stage('Test') {
            steps {
                sh 'npm test'
            }
            }      
    }
}