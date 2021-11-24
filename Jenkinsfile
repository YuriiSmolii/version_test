pipeline {
  agent {
    any
  }
  triggers{ cron( 0 15 * * * ) }
  options {
    disableConcurrentBuilds()
  }
  stages {
    stage('Foo') {
        steps {
            script {
                def now = new Date()
                println now.format("yyMMdd.HHmm", TimeZone.getTimeZone('UTC'))
            }
        } 
    }
  }
}