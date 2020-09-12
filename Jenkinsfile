pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.FILENAME = readfile 'name.txt'
                }
                echo "${env.FILENAME}"
            }
        }
    }
}
