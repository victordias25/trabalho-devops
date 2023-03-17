pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Exemplo') {
            steps {
                bat 'npm config ls'
            }
         }
        stage ('Build'){
            steps {
                bat 'npm install'
                bat 'npm install --no-fund core-js'         
            }
        }  
        stage('Install dependencies') {
            steps {
                bat 'npm install'
                bat 'npm run bowerInstall'
            }
        }
     
        stage('Test') {
            steps {
                bat 'npm test'
            }
        }      
        /*stage('Install dependencies') {
             steps {
                bat 'npm install'
                bat 'npm run bowerInstall'
             }
         }
        stage('Test') {
            steps {
                bat 'npm test'
            }
        }
        stage('Teste') {
            steps {
                sh 'chmod +x ./jenkins/scripts/test.sh'            
                sh './jenkins/scripts/test.sh'
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
        } */
    }
}


