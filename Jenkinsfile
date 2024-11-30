pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage('this is error stage') {
            steps {
                echo "This stage will fail with error code"
                error "ORA-01555"
            }
        }
    }
}