
pipeline {
    agent any
     triggers {
        githubPush()
    }
    tools {nodejs "node 15.6.0"}
    stages {
        

        stage('Prepare') {
            steps {
                sh 'npm --version'
                sh 'npm install'
                sh 'npm list'
            }
        }

        stage("Test") {
            steps {
                sh 'npm run nx -- run-many --target=test --all'
            }
        }

        stage("Lint") {
            steps {
                sh 'npm run nx -- run-many --target=lint --all'
            }
        }

        stage("Build") {
            steps {
                sh 'npm run nx -- run-many --target=build --all --prod'
            }
        }

        
       
    }
}