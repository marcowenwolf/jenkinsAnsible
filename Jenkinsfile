pipeline {
  agent none
  stages {
    stage('MetroAnsible') {
      steps {
        node(label: 'Waterhoen') {
          sh '''date
/sbin/lspci'''
        }

        ansiblePlaybook 'build.yml'
      }
    }
  }
}