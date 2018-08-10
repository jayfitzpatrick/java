pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        stage('logger') {sh "logger findme"}
        stage('write_file') {sh "echo>findme findme"}
        }
    }
}
