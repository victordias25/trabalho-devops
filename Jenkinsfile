pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage ('Build'){
            steps {
                bat 'npm install'       
            }
        }
    }
    stages ('Teste') {
        steps {
            sh './jenkins/scripts/test.sh'
        }
    }
}

