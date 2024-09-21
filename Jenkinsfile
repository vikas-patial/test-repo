pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh '''pwd
ls
sudo apt-get install -y apache2'''
      }
    }

    stage('build') {
      steps {
        echo 'hello'
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