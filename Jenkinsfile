pipeline {
    agent any
    
    tools {
        maven 'MAVEN'
        jdk 'JDK1.8'
    }
    stages {
        stage ('Initialize') {
            steps {
                echo "MAVEN_HOME = $MAVEN_HOME"
                echo "JAVA_HOME = $JAVA_HOME"
            }
        }
        
        stage('Build') {
            steps {
                echo 'this is a minimal build'
            }
         }
       }
     }
            
