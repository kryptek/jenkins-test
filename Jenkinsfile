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
    stage('Run script') {
      steps {
        parallel(
          "Run script": {
            sh '''pwd
uname -a
'''
            
          },
          "Eval?": {
            script {
              if (true) {
                this.binding.variables.each {k,v -> println "$k = $v"}
              }
            }
            
            
          }
        )
      }
    }
  }
}