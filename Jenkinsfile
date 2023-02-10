pipeline {

    agent any
        options {
                   disableConcurrentBuilds(abortPrevious: true)
                }
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        } 
        stage("timeout") {
            steps {
                timeout(time: 30, unit: 'MINUTES') {
                    input message: "does this look good"
                }
            }
        }        
    }
}

