pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage ('Build'){
            steps {
                bat 'npm install'       
            }
        }  
        stage('Test') {
            steps {
                bat 'chmod +x ./jenkins/scripts/test.sh'            
                bat './jenkins/scripts/test.sh'
            }                
        }       
    } 
}


