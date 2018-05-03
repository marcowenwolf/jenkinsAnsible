pipeline {
  agent any
    triggers {
        cron('H */4 * * 1-5')
    }
  stages {
    stage('MetroAnsible') {
      steps {
        node(label: 'Linux') {
          sh '''date
/sbin/lspci'''
        }

        node(label: 'Linux') {
          ansiblePlaybook '/home/marcwolf/tmp/nuage-metro-2.3.2/build.yml'
        }

      }
    }
  }
}
