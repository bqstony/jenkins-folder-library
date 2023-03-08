pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'

                echo "Triggered on branch ${BRANCH_NAME}"
                script{
                    def log = load "jenkins/log.groovy"
                    def shared = load "${pwd()}/jenkins/shared.groovy"

                    log.info("Hello groovy")
                    shared.doSomeStuff()
                }                
            }
        }
    }
}
