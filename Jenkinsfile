pipeline {
    agent any
    stages {
        stage ("Build Stage") {
            steps {
                echo "Entering Building Block"
                retry(3) {
                    echo "Welcome to jenkins"
                    error "testing retry block using error"
                }
                echo "***** After 3 retry's *****"
            }
        }
    }
}
