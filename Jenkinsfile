// Set a timeout period for the Pipeline run, after which Jenkins should abort the Pipeline
pipeline {
    agent {
        label "java-agent-slave"
    }
    stages {
        stage ("Build Stage") {
            steps {
                echo "Entering Building Stage"
                timeout(time: 10, unit: 'SECONDS') {
                    echo ("Sleeping 60 seconds")
                    sleep 60
                }
            }
        }
    }
}
