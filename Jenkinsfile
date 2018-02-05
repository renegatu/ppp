pipeline {
  agent {
    node {
      label 'pi2'
    }
    
  }
  stages {
    stage('stage1') {
      steps {
        echo 'ppp - stage unu'
      }
    }
    stage('stage2') {
      steps {
        sh 'uptime'
      }
    }
  }
}