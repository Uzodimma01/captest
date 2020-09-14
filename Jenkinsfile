pipeline {
    agent any
    stages {
        stage("foo") {
            steps {
                script {
                    env.FILENAME = readFile 'name.txt'
                }
                echo "Hello ${env.FILENAME}"
            }
        }
        stage("make dir") {
            steps {
                sh 'bash mkdir.sh'
                sh 'bash mktxt.sh'
            }
        }
        stage('Write file') {
            steps {
                sh 'bash ryt.sh'
            }
        }
    }
}
