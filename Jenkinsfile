pipeline {
    agent {
        label 'java-slave'
    }
    environment {
        name = 'KISHORE'
        schema = 'SPSOWNER'
    }
    stages {
        stage ('this is maven-stage: 1') {
            steps {
                echo "Welcome to ${name}"
                echo "This is ${schema}"
            }
        }
        stage ('this is second-stage') {
            environment {
                database = 'SPSCOREP'
            }
            steps {
                echo "welcome mr.${name}"
                echo "this is related to ${schema} schema"
                echo "database name is ${database}"
            }
        }
    }
}