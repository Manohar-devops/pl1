pipeline {
    agent {
        label "java-agent-slave"
    }
    stages {
        stage ("Build Stage") {
            steps {
                echo "This is 1st step under Build stage"
                sh "hostname -i"
            }
        }
        stage ("Scripted Stage") {
            steps {
                echo "This is 1st step under Scripted Stage"
                script {
                    echo "This is 2nd step under Scripted Stage"
                    def x = 10
                    if (x == 10) {
                        println ("Yes, the value is $x")
                    }
                    else 
                        println ("Enter the correct value")
                }
                sleep 10
            }
        }
        stage ("Sonar Stage") {
            steps {
                echo "This is 1st step under Sonar stage"
                echo "Code Quality is good, LGTM"
            }

        }
    }
}
