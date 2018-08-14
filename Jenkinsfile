pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('services') {
            steps {sh "sudo service docker start"}}
        stage('build') {
            steps {sh 'npm --version'} }
        stage('logger') {
            steps {sh "logger findme"} }
        stage('write_file') {
            steps { sh 'sudo service docker stop'
            sh "echo>findme findme"} }
    }
}
