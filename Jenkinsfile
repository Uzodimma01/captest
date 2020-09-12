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
    stages {
        stage("bar") {
            steps {
                script {
                    env.project_path = readFile 'path.txt'
                }
                echo "${env.project_path}"
            }
        }
    }
}
