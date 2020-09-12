pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.name = readFile('name.txt').trim()
                    env.path = readFile('path.txt').trim()
                }
                echo "${env.name}:${env.path}"
            }
        }
        stage("bar") {
            steps {
                echo "hello ${env.name}
            }
    }
}
