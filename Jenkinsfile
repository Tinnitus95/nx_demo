
pipeline {
    agent any
     triggers {
        githubPush()
    }
    stages {
        withNPM() {
            stage('build') {
                 steps {
                    sh 'npm --version'
                }
            }
        }
    }
}