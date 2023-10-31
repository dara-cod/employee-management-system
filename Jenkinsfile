pipeline {
    agent any
    tools {
        maven 'maven-3.6.3'
    }
    stages {
        stage('Maven build') {
            when {
                branch "main"
            }
            steps {
                sh "mvn clean package -DskipTests"
            }
        }
    }
}
