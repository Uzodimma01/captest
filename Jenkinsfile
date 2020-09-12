pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.FILENAME = readFile 'name.txt'
                }
                echo "${env.FILENAME}"
            }
        }
    }
}
