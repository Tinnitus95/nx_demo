
pipeline {
    agent any
     triggers {
        githubPush()
    }
    tools {nodejs "node 15.6.0"}
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}