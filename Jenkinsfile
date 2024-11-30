pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('This is JAVA-SLAVE: stage') {
            steps {
                script {
                    sh 'java -version'
                }
            }
        }
        stage ('This is executing from DOCKER-SLAVE: stage') {
            steps {
                script {
                    sh 'docker -version'
                }
            }
        }
    }
}