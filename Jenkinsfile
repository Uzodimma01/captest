pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.NAME = readFile 'path.txt'
                }
                echo "${env.NAME}"
            }
        }
    }
}
