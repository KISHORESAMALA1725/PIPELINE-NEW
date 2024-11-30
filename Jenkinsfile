pipeline {
    agent {
        label 'java-slave'
    }
    environment {
       NEXUS_CREDS = credentials('nexus_creds')
    }
    stages {
        stage ('this is credentials - stage') {
            steps {
                echo "nexus credentials are ${NEXUS_CREDS}"
                echo "username is ${NEXUS_CREDS_USR}"
                echo "password is ${NEXUS_CREDS_PSW}"
            }
        }
    }
}