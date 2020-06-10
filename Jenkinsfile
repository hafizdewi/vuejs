pipeline {
  agent any
  tools {nodejs "node" }
  stages {
    stage('Cloning Git') {
      steps {
        git credentialsId: 'hafizdewi', url: 'https://github.com/hafizdewi/vuejs.git'
      }
    }
    stage('Build') {
       steps {
         sh 'cd C:/Program Files (x86)/Jenkins/workspace/vuejenkins && cnpm install && npm run build'
       }
    }
  }
}