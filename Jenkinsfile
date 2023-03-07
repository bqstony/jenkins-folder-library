def log = load "${pwd()}/jenkins/log.groovy"
def shared = load "${pwd()}/jenkins/shared.groovy"

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    log.info("Hello groovy")
                }
                // Call method
                shared.doSomeStuff()
            }
        }
    }
}
