/*Jenkinsfile (Declarative Pipeline)*/
/* Requires the Docker Pipeline plugin */
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'node --version'
                sh 'npm ru ng build --prod --aot --sm --progress=false'
            }
        }
       stage('Test') {
       steps {
          sh 'npm ru ng test --progress=false --watch false'
        }}
      
    }
    }

