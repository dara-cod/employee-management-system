pipeline {
    agent any;
    stages {
        stage('Maven build') {
            when {
                "main"
            }
            steps {
                sh "mvn -s settings.xml clean deploy"
            }
        }
    }
}