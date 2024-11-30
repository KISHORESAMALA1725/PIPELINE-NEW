pipeline {
    agent {
        label 'java-slave'
    }
    tools {
        maven 'maven-3.8.8'
    }
    stages {
        stage ('this is maven-stage') {
            steps {
                script {
                    sh 'mvn -version'
                }
            }
        }
        stage (this is from autoinstaller maven stage){
            tools {
                maven 'maven-autoinstaller'
            }
            steps {
                script {
                    sh 'mvn -version'
                    sh 'java -version'
                }
            }
        }
    }

}