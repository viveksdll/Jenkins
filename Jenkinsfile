pipeline {
  agent any
  stages {
    stage('Checkout stage') {
      steps {
        git(url: 'https://github.com/viveksdll/django-todo-cicd.git', branch: 'main')
      }
    }

    stage('LOg') {
      steps {
        echo 'todo app'
      }
    }

  }
}