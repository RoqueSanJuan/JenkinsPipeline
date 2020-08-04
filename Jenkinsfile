pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build'
          }
        }

        stage('Test') {
          steps {
            sh 'Testing Chrome ${ChromeDriverPath}'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
  environment {
    ChromeDriverPath = '"C:\\Driver\\Chrome"'
  }
}