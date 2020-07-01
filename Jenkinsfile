pipeline {
  agent any
  stages {
    stage('echo') {
      parallel {
        stage('echo') {
          steps {
            echo 'hello from the trigger'
          }
        }

        stage('echo2') {
          steps {
            echo 'echo "hello2"'
          }
        }

      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}