pipeline {
  agent none
  stages {
    stage('MetroAnsible') {
      steps {
        node(label: 'Waterhoen') {
          sh '''date
/usr/sbin/lspci'''
        }

      }
    }
  }
}