
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    def log = load "${pwd()}/jenkins/vars/log.groovy"
                    log.info("Hello groovy")
                }
            }
        }
    }
}
