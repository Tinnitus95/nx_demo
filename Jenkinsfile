
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
                sh 'npm install @nrwl/cli@11.0.0'
                sh 'npm -v @angular/cli'
            }
        }
       
    }
}