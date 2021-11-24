pipeline {
  agent any
  triggers{ cron('13 12 * * *') }
  stages {
    stage('Foo') {
        steps {
            script {
                def now = new Date()
                println now.format("H:mm", TimeZone.getTimeZone('UTC'))
            }
        } 
    }
  }
}