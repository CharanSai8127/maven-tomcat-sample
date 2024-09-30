pipeline { 
    agent any  
    
    tools {
        jdk 'jdk 17'
        maven 'maven 3'
    }

    stages {
        stage('Git-checkout') {
            steps {
                git 'https://github.com/CharanSai8127/maven-tomcat-sample.git'
            }
        }
        
         stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
         stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
