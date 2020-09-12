pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                sh '''
                set +x 
                echo "Hello plus"
                '''
                sh '''
                set +x 
                bash ./export.sh
                '''
                sh '''
                set +x 
                export project_name
                '''
                sh '''
                set +x 
                project_path="$(<./path.txt)":$project_name
                '''
                sh '''
                set +x 
                bash test.sh
                '''
                sh '''
                set +x 
                bash echo.sh
                '''
                sh '''
                set +x 
                echo ${project_path}
                '''
                sh '''
                set +x 
                echo ${project_name}
                '''
            }
        }
    }
}
