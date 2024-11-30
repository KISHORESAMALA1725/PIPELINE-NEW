pipeline {
    agent {
        label 'docker-slave'
    }
    stages{
        stage ('this is docker-slave') {
            steps {
                options {
                    timeout (time: 3, unit: 'seconds')
                }
                echo "timeout-occurred, please retry again"
                sleep 30
            }
        }
    }
}