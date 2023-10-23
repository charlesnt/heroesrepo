/*Jenkinsfile (Declarative Pipeline)*/
/* Requires the Docker Pipeline plugin */
pipeline {
    agent any
    stages {
        stage('build') {
            steps {
               nodejs('node@8.12.0'){
                sh 'node --version'
                sh 'npm install'
               }
            }
        }
       stage('Test') {
       steps {
          nodejs('node@8.12.0'){
          sh 'npm run ng test --progress=false --watch false'
        }}}
      
    }
    }

