pipeline {
    environment {
    //DatosProyecto
        projectName = 
        buildCommand = 
        compile = 
        publishToTEST = 
        publishToPRO = 
    //SonarQube
        sources = 
        projectKey =
        scannerHome = 
    }
    agent {
        label '' //set agent
    }
    stages {
        stage('Install postman'){
          npm install -g newman
        }
        
        
        stage('Build & Unit Test'){
            steps {  
                
            }
        }
        stage('SonarQube analysis') {
            steps {
                
            }
        }
        stage('Connect Azure') {
            steps {
                
            }
        }
        stage('Deploy') {
            parallel {
                //stages to deploy to azure
            }
        }
        stage('Disconnect Azure') {
            steps {
                
        }
    }
    post {
        always {
            echo 'Finalizado. Limpiando workspace'
            deleteDir()
        }
    }

