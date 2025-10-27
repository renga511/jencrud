pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/renga511/jencrud.git'
            }
        }
        stage('Build HTML') {
            steps {
                bat 'dir'
            }
        }
        stage('Display Link') {
            steps {
                script {
                    echo "✅ CRUD App Ready!"
                    echo "<a href='file:///C:/ProgramData/Jenkins/.jenkins/workspace/${env.JOB_NAME}/crud.html' target='_blank'>Open CRUD App</a>"
                }
            }
        }
    }
}
