
pipeline {
    agent any
     triggers {
        githubPush()
    }
    tools {nodejs "node"}
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
            }
        }
    }
}