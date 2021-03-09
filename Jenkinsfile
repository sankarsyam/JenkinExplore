pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
               echo "$GIT_BRANCH"
            }
        }
         stage('Build') {
            steps {
               npm run build
            }
        }
         stage('Run Test') {
            steps {
               npm run test
            }
        }
    }
}