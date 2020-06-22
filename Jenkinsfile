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
                   bat " mvn clean install"
            }
         }
        Stage('Deploy') {
            steps{
                deploy adapters: [tomcat7(credentialsId: '918843d5-4736-4445-a5c0-d44a49a7fbc5', path: '', url: 'http://localhost:8085/')], contextPath: 'TomcatMavenApp', war: '**/*.war'
       }
     }
    }
}
            
