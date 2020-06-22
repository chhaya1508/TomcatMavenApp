pipeline {
    agent any
    
    tools {
        maven 'MAVEN'
        jdk 'JDK1.8'
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }
        
        stage('Build') {
            steps {
                echo 'thi is a minial build'
            }
         }
       }
     }
            
