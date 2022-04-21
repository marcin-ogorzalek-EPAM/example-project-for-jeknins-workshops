pipeline {
    agent any
    tools {
      maven 'My Maven'
      jdk 'my-jdk'
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
