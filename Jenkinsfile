/*Jenkinsfile (Declarative Pipeline)*/
/* Requires the Docker Pipeline plugin */
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'node --version'
                sh 'ng build --prod --aot --sm --progress=false'
            }
        }
       stage('Test') {
      
          sh 'ng test --progress=false --watch false'
        }
      
    }
    }

