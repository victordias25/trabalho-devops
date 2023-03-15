pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage ('Build'){
            steps {
                bat 'npm install'       
            }
        }
        stage('Teste') {
            steps {
                bat './jenkins/scripts/test.sh'
             }
        }
    }  
}

