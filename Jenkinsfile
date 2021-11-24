pipeline {
  agent any
  triggers{ cron('00 14 * * *') }
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