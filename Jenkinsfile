pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', url: 'https://github.com/ridhima13121989/day1.git'

      }
    }

    stage('Deploy to Nginx') {
      steps {
        sh '''
          rm -rf /var/www/html/*
          cp -r . /var/www/html/
          ls -la /var/www/html
        '''
      }
    }
  }
}
