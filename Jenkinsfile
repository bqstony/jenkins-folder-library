def log = load "${pwd()}/jenkins/vars/log.groovy"

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                log.info("Hello groovy")
            }
        }
    }
}
