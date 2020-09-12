pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                sh 'echo "Hello plus"'
                sh 'bash ./export.sh'
                sh 'export project_name'
                sh 'project_path="$(<./path.txt)":$project_name'
                sh 'bash test.sh'
                sh 'bash echo.sh'
                sh 'echo $project_path'
                sh 'echo $project_name'
            }
        }
    }
}
