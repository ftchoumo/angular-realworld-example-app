pipeline {
    agent any 
    stages {
        stage('cloning the rpo') {
 #           agent { docker 'maven:3.8.1-adoptopenjdk-11' } 
            steps {
                git clone 'https://github.com/ganatan/angular-starter.git'
            }
        }
        stage('Go to the project root') {
#            agent { docker 'openjdk:8-jre' } 
            steps {
              cd 'angular-starter'
            }
        }
       stage('Install angular') {
            steps {
              npm 'install'
            }
        }
       stage('Install angular') {
            steps {
              npm 'start'
            }
        }      
    }
}




