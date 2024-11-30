pipeline {
    agent {
        label 'docker-slave'
    }
    stages{
        stage ('this is docker-slave') {
            steps {
                    timeout (time: 3, unit: 'SECONDS')
                    echo "timeout-occurred, please retry again"
                    sleep 30
            }
        }
    }
}