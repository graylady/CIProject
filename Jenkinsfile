pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }
       stage('Test ') {
            steps {
                bat 'npm run test --  --coverage'
             }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
   