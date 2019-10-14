pipeline {
    agent none
    stages {
        stage('Docker Test') {
            agent { docker 'hello-world' }
            steps {
                echo 'Hello from Docker'
            }
       }
        stage('Example Build') {
            agent { docker 'maven:3-alpine' }
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            agent { docker 'openjdk:8-jre' }
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
