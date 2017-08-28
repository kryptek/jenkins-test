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
    stage('Runnit') {
      steps {
        script {
          script {
            
            def tests = ['a', 'b', 'c']
            for (int i = 0; i < tests.length; i++) {
              stage("Test ${tests[i]}") {
                sh 'pwd'
              }
            }
            
          }
        }
        
      }
    }
  }
}