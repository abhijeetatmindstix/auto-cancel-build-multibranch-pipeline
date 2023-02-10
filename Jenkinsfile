pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage("cancel-previous-build") {
            steps {
                cancelUnwantedBuilds()
            }
        }        
    }
}

