pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.project_name = readFile 'name.txt'
                }
                echo "${env.project_name}"
            }
        }
    }
}
