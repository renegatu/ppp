pipeline {
  agent {
    node {
      label 'pi2'
    }
    
  }
  stages {
    stage('stage1') {
      environment {
        vara1 = '000'
      }
      parallel {
        stage('stage1') {
          steps {
            echo 'ppp - stage unu'
          }
        }
        stage('and more') {
          steps {
            sh 'uname -a'
            sleep 5
            pwd()
          }
        }
      }
    }
    stage('stage2') {
      steps {
        sh 'uptime'
        sh 'echo "variable value vara1 is ..$vara1.."'
      }
    }
  }
}