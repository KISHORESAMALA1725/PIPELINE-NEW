pipeline {
    agent {
        label 'docker-slave'
    }
    environment {
        database='JAVA'
    }
    stages {
        stage ('this is build stage'){
            when {
                environment name: 'database', value: 'JAVA'
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