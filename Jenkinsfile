pipeline {
    agent { docker { image 'maven:3.9.2-eclipse-temurin-11' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Run') {
            steps {
                sh 'java -jar target/demo-jenkins-0.0.1-SNAPSHOT.jar' // Run the Spring Boot application
            }
        }
    }
}
