pipeline {
    agent {
        label "java-agent-slave"
    }
    stages {
        stage ("Build Stage") {
            steps {
                echo "Building application"
                sh 'hostname -i'
            }
        }
        stage ("Scripting Stage") {
            steps {
                echo "This is 1st step from 2nd stage"
                script {
                    def x = 10
                    if (x == 10) {
                        println ("Yes, the value is $x")
                    }
                    else
                        println ("Enter the correct value")
                }
            }
        }
        stage ("Sonar Stage") {
            steps {
                echo ("Code Quality is good, LGTM")
            }
        }

    }
}
