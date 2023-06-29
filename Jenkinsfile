pipeline {
    agent any;
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
