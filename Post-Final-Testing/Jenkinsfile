pipeline {
    agent any
    stages {
         stage('Clone repository') { 
            steps { 
                checkout scm
            }
        }

        stage('Build') { 
            steps { 
                script{
                 app = docker.build("testapp-cicd")
                }
            }
        }
        stage('Test'){
            steps {
                 echo 'Empty'
            }
        }
        stage('Deploy') {
            steps {
                script{
			withCredentials([aws(credentialsId: "01cd5edb-761a-4bdf-8e2c-21505463c9ai")]) {
			
			}
                    }
                }
            }
        }
    }
