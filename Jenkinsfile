/* Requires the Docker Pipeline plugin */
pipeline {
    agent { 
        docker { 
            image 'maven:3.10.0-eclipse-temurin-21-alpine'
            args '-v C:/Users/wenni/.jenkins/workspace/FirstPipeline_main:/workspace -w /workspace'
        }
    }
    stages {
        stage('build') {
            steps {
                bat 'mvn --version'
            }
        }
    }
}