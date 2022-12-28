pipeline {
  agent any
  stages {
    stage('Git Pull') {
      steps {
        git(url: 'https://github.com/mdrajibkhan/time-track.git', branch: 'master', poll: true)
      }
    }

    stage('Building Application') {
      steps {
        sh 'mvn clean install'
      }
    }

  }
}