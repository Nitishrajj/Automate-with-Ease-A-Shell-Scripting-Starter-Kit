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
                bat 'python3 basic.py'
            }
        }
    }
}
