pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.name = readFile 'name.txt' 
                    env.path = readFile 'path.txt'
                }
                echo "${env.path}${env.name}"
                sh 'echo "hello"'
            }
        }
    }
}
