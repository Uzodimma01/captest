pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.NAME = readFile 'output.txt'
                }
                echo "${env.FILENAME}"
            }
        }
    }
}
