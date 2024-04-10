 pipeline {     
    agent any
    
    tools {
        jdk 'jdk17'
        maven 'maven'
    } 

    stages {
        
         
        stage('Compile') {
            steps {
            sh  "mvn compile"
            }
        }
        
        stage('tests') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
