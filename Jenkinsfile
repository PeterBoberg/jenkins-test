pipeline {
    agent any
    stages {
        stage('Cleaning ') {
            steps {
                sh "echo 'STARTING BUILD'"
            }
        }

        stage('build') {
            steps {
                sh "mvn clean package"
            }
        }

        stage('Say hello') {
            steps {
                sh "echo 'Hello there'"
            }
        }
    }
}