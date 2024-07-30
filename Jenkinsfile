pipeline { 
    agent {
        label 'slave'
    }
    
    tools {
        jdk 'jdk 17'
        maven 'maven'
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
