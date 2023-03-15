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
        stage('Deliver for development') {
            when {
                branch 'development'
            }
            steps {
                sh 'chmod +x ./jenkins/scripts'
                sh './jenkins/scripts/deliver.sh'
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                sh './jenkins/scripts/kill.sh'
            }
        }
        stage('Deploy for production') {
            steps {
                sh 'chmod -R +x ./jenkins/scripts'
                sh './jenkins/scripts/deliver.sh'
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                sh './jenkins/scripts/kill.sh'
            }       
        } 
    }
}


