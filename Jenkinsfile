# On failure, retry the entire Pipeline the specified number of times. For example: options { retry(3) }
pipeline {
    agent any
    stages {
        stage ("Build Stage") {
            steps {
                echo "Entering Build Stage"
                retry(3) {
                    echo "Welcome to Jenkins"
                    error "Testing retry block using error"
                }
            }
        }
    }
}
