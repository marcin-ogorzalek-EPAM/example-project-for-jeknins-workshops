pipeline {
//     agent any
//     tools {
//       maven 'My Maven'
//       jdk 'my-jdk'
//     }
    agent {
        docker { image 'maven:3.6.3' }
    }
    environment {
        DOCKER_HOST = 'unix:///run/user/1000/docker.sock'
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
