 
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build Production files') {
            steps {
                bat 'npm run build'
            }
        }
       stage('test vad som händer') {
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