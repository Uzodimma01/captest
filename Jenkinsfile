pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.name = readFile 'name.txt' 
                    env.path = readFile 'path.txt'
                }
                echo "${env.name}"
                echo "${env.path}"
                echo "${env.proj}"
                echo "name/${env.name}.concat(${env.path})"
            }
        }
    }
}
