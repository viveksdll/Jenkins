pipeline {
  agent any
  stages {
    stage('Checkout stage') {
      steps {
        git(url: 'https://github.com/viveksdll/django-todo-cicd.git', branch: 'develop')
      }
    }

    stage('error') {
      parallel {
        stage('error') {
          steps {
            echo 'Test Stage'
          }
        }

        stage('Install') {
          steps {
            sh '''RUN pip install django==3.2
RUN python manage.py'''
          }
        }

      }
    }

  }
}