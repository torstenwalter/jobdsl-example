pipeline {
    agent any
    stages {
        stage('configure jobs') {
            steps {
                jobDsl failOnMissingPlugin: true, removedConfigFilesAction: 'DELETE', removedJobAction: 'DISABLE', removedViewAction: 'DELETE', targets: 'jobs/**/*.grooxy', unstableOnDeprecation: true
            }
        }
    }
}
