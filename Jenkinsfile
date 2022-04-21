pipeline {
//     agent any
//     tools {
//       maven 'My Maven'
//       jdk 'my-jdk'
//     }
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
