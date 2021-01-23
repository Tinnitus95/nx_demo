
pipeline {
    agent any
     triggers {
        githubPush()
    }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}