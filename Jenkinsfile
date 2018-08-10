pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {sh 'npm --version'} }
        stage('logger') {
            steps {sh "logger findme"} }
        stage('write_file') {
            steps {sh "echo>findme findme"} }
    }
}
