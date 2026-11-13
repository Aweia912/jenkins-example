/* Requires the Docker Pipeline plugin */
pipeline {
    agent { 
        docker { 
            image 'maven:3.10.0-eclipse-temurin-21-alpine'
            args '-v C:/Users/tlkjl/.jenkins/workspace/My-Pipeline_main:/workspace -w /workspace'
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}