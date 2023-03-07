pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    def log = load "${pwd()}/jenkins/log.groovy"
                    def shared = load "${pwd()}/jenkins/shared.groovy"

                    log.info("Hello groovy")
                    shared.doSomeStuff()
                }                
            }
        }
    }
}
