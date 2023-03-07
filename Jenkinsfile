
pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    log.info("Hello groovy")
                    def log = load "${pwd()}/jenkins/vars/log.groovy"
                }
            }
        }
    }
}
