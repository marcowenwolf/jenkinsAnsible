pipeline {
  agent any
  stages {
    stage('MetroAnsible') {
      steps {
        node(label: 'Waterhoen') {
          sh '''date
/sbin/lspci'''
        }

        node(label: 'Waterhoen') {
          ansiblePlaybook '/home/marcwolf/tmp/nuage-metro-2.3.2/build.yml'
        }

      }
    }
  }
  triggers {
    cron('H */4 * * 1-5')
  }
}