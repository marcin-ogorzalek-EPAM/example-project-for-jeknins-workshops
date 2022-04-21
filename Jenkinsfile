pipeline {
    agent any
    tools {
      maven 'My Maven'
      jdk 'my-jdk'
    }
    options {
        buildDiscarder(logRotator(daysToKeepStr: '1', numToKeepStr: '5', artifactDaysToKeepStr: '2', artifactNumToKeepStr: '1'))
    }
    stages {
        stage('env info') {
            steps {
                sh 'mvn --version'
                sh 'java --version'
            }
        }
        stage('build') {
            steps {
                sh 'mvn compile'
                sh 'mvn package'
            }
        }
        stage('sleep') {
            steps {
                sleep(time: 1, unit: 'MINUTES')
                echo('Hello world')
            }
        }
    }
}
