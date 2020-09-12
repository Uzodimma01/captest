pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.project_name = readfile 'path.txt'
                }
                echo "Hello ${env.project_name}"
            }
        }
    }
}
