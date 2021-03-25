pipeline {
  agent any
  stages {
    stage('Print') {
      parallel {
        stage('Print') {
          steps {
            echo 'Pipeline initiated'
          }
        }

        stage('Build') {
          steps {
            echo 'Build Started'
          }
        }

        stage('SonarQube - Code Quality') {
          steps {
            echo 'Testing code quality'
          }
        }

        stage('TestProject - Testing') {
          steps {
            echo 'UAT/UI testing started'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy to Development'
      }
    }

  }
}