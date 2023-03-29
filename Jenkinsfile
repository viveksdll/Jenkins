pipeline {
  agent any
  stages {
    stage('Checkout stage') {
      steps {
        git(url: 'https://github.com/viveksdll/django-todo-cicd.git', branch: 'develop')
        echo 'Checkout'
      }
    }

    stage('Build') {
      steps {
        echo 'Build Stage'
        sh '''RUN pip install django==3.2
RUN python manage.py'''
      }
    }

    stage('deploy') {
      steps {
        echo 'Deploy stage'
        sh 'Python manage.py'
      }
    }

  }
}