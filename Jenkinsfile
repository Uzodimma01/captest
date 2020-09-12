pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.FILENAME = readFile 'name.txt'
                }
                sh "k=${env.FILENAME}"
                sh "echo $k"
            }
        }
    }
}
