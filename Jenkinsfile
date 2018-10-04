pipeline {
    agent any
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!'
            }
        }

        stage('build') {
            steps {
                mvn clean package
            }
        }
    }
}