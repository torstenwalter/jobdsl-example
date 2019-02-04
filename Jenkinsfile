pipeline {
    agent any
    stages {
        stage('configure jobs') {
            steps {
                jobDsl failOnMissingPlugin: true, removedConfigFilesAction: 'DELETE', removedJobAction: 'DISABLE', removedViewAction: 'DELETE', targets: 'jobs/**/*.groovy', unstableOnDeprecation: true
            }
        }
    }
}
