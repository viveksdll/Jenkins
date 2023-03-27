pipeline {
  agent any
  stages {
    stage('Checkout stage') {
      steps {
        git(url: 'https://github.com/viveksdll/django-todo-cicd.git', branch: 'develop')
      }
    }

    stage('error') {
      steps {
        echo 'Test Stage'
      }
    }

  }
}