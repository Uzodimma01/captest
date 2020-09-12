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
    stage("bar") {
        steps {
            script {
                env.path = readfile 'path.txt'
            }
            echo "${env.path}"
        }
    }
}
