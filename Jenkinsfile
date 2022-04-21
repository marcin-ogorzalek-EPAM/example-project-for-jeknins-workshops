pipeline {
    agent any
    tools {
      maven 'My Maven'
      jdk 'my-jdk'
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
    }
}
