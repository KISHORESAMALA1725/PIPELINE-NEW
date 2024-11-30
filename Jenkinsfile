pipeline {
    agent any
    environment {
        database="DOCKER"
    }
    stages {
        stage ('this is build stage'){
            when {
                environment name: 'database', value: 'DOCKER'
            }
            steps {
                echo "this will get executed in docker-slave machine"
                script {
                    'sh hostname'
                }
            }
        }
    }
}