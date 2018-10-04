pipeline {
    agent any
    options([pipelineTriggers([pollSCM('H * * * *')])])
    stages {
        stage('Clone repo') {
            steps {
                sh "mvn clean"
            }
        }

        stage('build') {
            steps {
                sh "mvn package"
            }
        }

        stage('Say hello') {
            steps {
                sh "echo 'Hello there'"
            }
        }
    }
}