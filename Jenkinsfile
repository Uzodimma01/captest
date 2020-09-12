pipeline {
    agent any
    stages {
        stage("Foo") {
            steps {
                script {
                    env.name = readfile("name.txt").trim()
                    env.path = readfile("path.txt").trim()
                }
            }
        }
    }
}
