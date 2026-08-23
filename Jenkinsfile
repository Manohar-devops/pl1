pipeline {
    agent node
    stages {
        stage ("Build Stage") {
            agent {
                labels "java-agent-slave"
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
