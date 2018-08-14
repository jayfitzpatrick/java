pipeline {
stage('services') {
    steps {sh 'sudo service docker start'}}
agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {sh 'npm --version'} }
        stage('logger') {
            steps {sh 'logger findme'} }
        stage('write_file') {
            steps { sh 'sudo service docker stop'
            sh "echo>findme findme"} }
    }
}
