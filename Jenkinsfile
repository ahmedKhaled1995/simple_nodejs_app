pipeline {
    agent any

    stages {
        stage('Getting Repo Files') {
            steps {
                git branch: 'main', credentialsId: 'github_token', url: 'https://github.com/ahmedKhaled1995/simple_nodejs_app.git'
            }
        }
        
        stage('Building Code') {
            steps {
                sh "docker build -t mynodeapp:v1.0 ."
            }
        }
    }
}
