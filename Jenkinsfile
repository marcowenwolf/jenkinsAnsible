pipeline {
  agent {
    node {
      label 'Linux'
    }

  }
  stages {
    stage('') {
      steps {
        node(label: 'Linux') {
          ansiblePlaybook 'vsd_predeploy.yml'
        }

      }
    }
  }
}