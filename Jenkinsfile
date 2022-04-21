pipeline {
//     agent any
//     tools {
//       maven 'My Maven'
//       jdk 'my-jdk'
//     }
    agent { docker { image 'maven:3.6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
