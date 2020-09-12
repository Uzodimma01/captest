pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.project_name = readfile 'name.txt'
                }
                echo "${env.project_name}"
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
}
