pipeline {
    environment {
    //DatosProyecto
        projectName = "test"
        buildCommand = ""
        compile = ""
        publishToTEST = ""
        publishToPRO = ""
    //SonarQube
        sources = ""
        projectKey = ""
        scannerHome = ""
    }
    agent any
    stages {
	stage('Newman run'){
		newman run 'Mule API Manager instance creation.postman_collection.json'
	}
	    /*
        stage('Build & Unit Test'){
            steps {  
                ""
            }
        }
        stage('SonarQube analysis') {
            steps {
                ""
            }
        }
        stage('Connect Azure') {
            steps {
                ""
            }
        }
        stage('Deploy') {
            parallel {
                //stages to deploy to azure
		    ""
            }
        }
        stage('Disconnect Azure') {
            steps {
                ""
        }
		}	
		*/
    post {
        always {
            echo 'Finalizado. Limpiando workspace'
            deleteDir()
        }
    }
}
}
