pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage ('Build'){
            steps {
                sh 'cd .\webapi\ '
                bat 'npm install'       
            }
        }
    }
}

