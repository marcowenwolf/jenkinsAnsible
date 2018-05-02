pipeline {
  agent {
    node {
      label 'Linux'
    }

  }
  stages {
    stage('MetroBuildVSD') {
      steps {
        node(label: 'laptop') {
          ansiblePlaybook 'vsd_predeploy.yml'
        }

      }
    }
  }
}