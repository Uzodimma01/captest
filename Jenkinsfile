pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.FILENAME = readfile 'path.txt'
                }
                echo "Hello ${env.FILENAME}"
            }
        }
    }
}
