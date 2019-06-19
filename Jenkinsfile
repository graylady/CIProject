 
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build Production files') {
            steps {
                sh 'npm run build'
            }
        }
       stage('test it') {
            steps {
                sh 'npm run test --  --coverage'
             }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}