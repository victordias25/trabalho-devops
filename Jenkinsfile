pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage ('Build'){
            steps {
                bat 'npm install'
                bat 'npm install nodemon'
                bat 'npm run star'
            }
        }
    }
}

