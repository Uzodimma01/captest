pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.name = readFile 'path.txt' 
                    env.path = readFile 'path.txt'
                }
                sh "echo "${env.path}${env.name}""
            }
        }
    }
}
