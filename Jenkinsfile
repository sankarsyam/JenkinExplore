pipeline {
     agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Verify Branch') {
            steps {
               echo "$GIT_BRANCH"
            }
        }
         stage('NPM Install') {
            steps {
               sh 'npm install' 
            }
        }
         stage('Run Test') {
            steps {
               sh 'npm run test' 
            }
        }
    }
}