pipeline {
    agent {
        label 'docker-slave'
    }
    stages {
        stage ('this is retry-stage') {
            steps {
                retry 5{
                    error "this is the error code ORA-01555"
                    echo "this is error code"
                }
            }
        }
    }
}