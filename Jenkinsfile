pipeline {
    agent any

    stages {
        stage('Hello World') {
            steps {
                echo 'Hello, World!'
            }
        }
        stage('Running python file'){
            steps {
                bat 'python basic.py'
            }
        }
    }
}
