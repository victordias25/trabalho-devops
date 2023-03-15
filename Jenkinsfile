pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage ('Build'){
            steps {
                bat 'cd webapi'
                bat 'npm install'       
            }
        }
    }
}

