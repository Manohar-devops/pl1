pipeline {
    agent none
    stages {
        stage "Build Stage" {
            agent {
                label "java-agent-slave"
            }
            steps {
                echo "This is a java node app"
                sh hostname -i
            }
        }
        stage "Scripted Stage" {
            agent {
                label "java-agent-slave"
            }
            steps {
                echo "Scripting in the java node app"
                script {
                    def x = 10
                    if x == 10
                       println ("Yes, the no. is $x")
                    else {
                        println ("Enter the correct value")
                    }
                }
            }
        }
        stage "Sonar Stage" {
            agent {
                label "node-agent-slave"
            }
            steps {
                echo "This is node app"
            }
        }

    }
}
