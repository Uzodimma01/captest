pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.name = readFile 'name.txt':'path.txt'
                    env.path = readFile 'path.txt'
                }
                echo "${env.path}${env.name}"
            }
        }
    }
}
