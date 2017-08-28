pipeline {
  agent any
  stages {
    stage('Provision Stack') {
      steps {
        parallel(
          "Provision Stack": {
            sh '''uptime
date +%s
sleep 5
date +%s'''
            
          },
          "Provision Stack2": {
            sh '''uptime
date +%s
sleep 5
date +%s'''
            
          },
          "Provision Stack3": {
            sh '''uptime
date +%s
sleep 5
date +%s'''
            
          }
        )
      }
    }
  }
}