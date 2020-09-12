pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.name = readFile 'name.txt' 
                    env.path = readFile 'path.txt'
                    env.proj = "name/${env.name}/${env.path}"
                }
                echo "${env.name}"
                echo "${env.path}"
                echo "${env.proj}"
            }
        }
    }
}
