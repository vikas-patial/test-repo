pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd
ls
apt-get install -y apache2'''
      }
    }

    stage('build') {
      steps {
        input(ok: 'yes', message: 'give input')
      }
    }

    stage('deploy-test') {
      steps {
        sleep(time: 5, unit: 'SECONDS')
      }
    }

    stage('deploy-prod') {
      steps {
        echo 'done !'
      }
    }

  }
}