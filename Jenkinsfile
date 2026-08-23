// Set a timeout period for the Pipeline run, after which Jenkins should abort the Pipeline
pipeline {
    agent {
        label "java-agent-slave"
    }
    stages {
        stage ("Build Stage") {
            steps {
                echo "Entering Building Stage"
                timeout(time: 5, unit: 'SECONDS')
            }
        }
    }
}
