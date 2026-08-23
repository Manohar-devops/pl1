pipeline {
    agent none
    stages {
        stage ("This is 1st Stage") {
            agent {
                label "java-agent-slave"
            }
            steps {
                echo "Welcome to Jenkins pipelines"
                echo "This is Java App"
            }
        }
        stage ("This is 2nd stage") {
            agent {
                label "node-agent-slave"
            }
            steps {
                echo "Pipeline is succeded"
                echo "This is Node App"
            }
        }
    }
}
