def deploy_date = (new Date()).format("YYYYMMdd-hh:mm:ss", TimeZone.getTimeZone('localtime'))
pipeline {
    agent any
    stages {
        stage('stage 1') {
            steps {
                sh "echo ${deploy_date}"
                sh "echo ${currentBuild.startTimeInMillis}"   
                sh "/bin/date -d @${currentBuild.startTimeInMillis}"        
            }
        }
	}
}