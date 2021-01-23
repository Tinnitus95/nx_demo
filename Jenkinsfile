
pipeline {
    agent any
     triggers {
        githubPush()
    }
    withNPM() {
        stages {
        
            stage('build') {
                steps {
                    sh 'npm --version'
                }
            }
        }
    }
}