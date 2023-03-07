def log = load "${pwd()}/jenkins/vars/log.groovy"

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    log.info("Hello groovy")
                }
            }
        }
    }
}
