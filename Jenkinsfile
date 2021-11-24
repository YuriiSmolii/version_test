pipeline {
  agent any
  triggers{ cron('15 13 * * *') }
  options {
    disableConcurrentBuilds()
  }
  stages {
    stage('Foo') {
        steps {
            script {
                def now = new Date()
                println now.format("Hmm", TimeZone.getTimeZone('UTC+2'))
            }
        } 
    }
  }
}