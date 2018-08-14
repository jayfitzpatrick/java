  pipeline  {
    agent none
      stages {
          stage('services')
            steps {sh 'sudo service docker start'
          agent { docker { image 'node:6.3' }
//              stage('build') {
//            steps {sh 'npm --version'} }
//        stage('logger') {
//            steps {sh 'logger findme'} }
//        stage('write_file') {
//            steps { sh "echo>findme findme"} }
//        stage('cleanup_services') {
//                steps { sh 'sudo service docker stop'} }
    }
  }
}
}
