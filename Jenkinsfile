pipeline {
  agent {
    node {
      label 'Waterhoen'
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