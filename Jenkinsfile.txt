pipeline {
    agent any
    
    environment{
        PROJECT_NAME="Neptun"
        
    }

    stages {
        stage('Build') {
            steps {
                echo "Start Building project ${PROJECT_NAME}"
            }
        }
        stage('Test'){
            steps{
                echo 'Start Testing'
                bat "dir"
            }
        }
        stage('Deploy'){
            steps{
                echo 'Start Deploying'
            }
        }
    }
}
