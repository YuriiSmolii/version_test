pipeline {
  agent any
  triggers{ cron('45 13 * * *') }
  options {
    disableConcurrentBuilds()
  }
  stages {
    stage('Foo') {
        steps {
            script {
                def now = new Date()
                println now.format("H:mm", TimeZone.getTimeZone('UTC+2'))
            }
        } 
    }
  }
}