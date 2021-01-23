
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
                sh 'npm install'
                sh 'npm list'
            }
        }
        stage('test') {
            steps {
                sh 'npm run nx -- run-many --target=test --all'
            }
        }

        stage('affected test') {
            sh 'npm run affected:test'
        }
       
    }
}