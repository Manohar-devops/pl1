pipeline {
    agent none
    stages {
        stage ("Build Stage") {
            agent {
                label "java-agent-slave"
            }
            steps {
                echo "Building the artifact"
            }
        }
        stage ("Sonar Stage") {
            agent {
                label "node-agent-slave"
            }
            steps {
                echo "Code quality is good, LGTM"
            }
        }
    }
}
