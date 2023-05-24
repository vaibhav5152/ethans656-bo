pipeline {
  agent any
  stages {
    stage('fetch code') {
      steps {
        git(url: 'https://github.com/vaibhav5152/ethans656-bo.git', branch: 'main')
      }
    }

    stage('install apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('deploy') {
      steps {
        sh 'sudo cp -R * /var/www/html'
      }
    }

  }
}