pipeline {
    agent any

    stages {
        
        stage('Getting Repo files') {
            steps {
                git branch: "${GIT_BRANCH}", credentialsId: 'github', url: 'https://github.com/ahmedKhaled1995/simple_nodejs_app.git'
            }
        }
        
        stage('Listing repo directory') {
            steps {
                sh '''
                    ls
                    echo "${GIT_BRANCH}"
                '''
            }
        }
    }
    
}
