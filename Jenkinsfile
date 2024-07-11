pipeline {
    agent any
    tools {
          maven "maven-3.6.3"
    }
    stages {
        stage ("Maven Clean") {
            when {
                branch "main"
            }
            steps {
                  sh "mvn clean"
            }
        }
        stage("Maven Build") {
            when {
                  branch "main"
            }
            steps {
                sh "mvn package -DskipTests"
                sh "mkdir pastateste"
            }
        }
    }
}
