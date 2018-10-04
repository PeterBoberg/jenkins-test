pipeline {
    agent any
    stages {
        stage('Clone repo') {
            steps {
                sh "rm -rf jenkins-test"
                sh "git clone https://github.com/PeterBoberg/jenkins-test.git"
                sh "mvn clean -f jenkins-test"
            }
        }

        stage('build') {
            steps {
                sh "mvn package -f jenkins-test"
            }
        }

        stage('Say hello') {
            steps {
                sh "echo 'Hello there'"
            }
        }
    }
}