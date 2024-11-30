pipeline {
    agent {
        label 'docker-slave'
    }
    stages {
        stage ('This is first stage') {
            steps {
                script {
                    def courses = 'DevOps'
                    if (courses == 'DevOps')
                    println ("Welcome to ${courses} - course")
                    else
                    println ("Please enroll to ${courses} now")
                }
            }
        }
    }
}