pipeline {
    agent {
        label "java-agent-slave"
    }
    stages {
        stage "Build Stage" {
            steps {
                echo "Building application"
                sh hostname -i
            }
        }
        stage "Scripted Stage" {
            steps {
                echo "Scripting in the java node app"
                script {
                    def x = 10
                    if (x == 10) {
                        println ("Yes, the no. is $x")
                    }
                    else {
                        println ("Enter the correct value")
                    }
                }
            }
        }
        stage "Sonar Stage" {
            steps {
                echo "Doing Sonar"
            }
        }

    }
}
