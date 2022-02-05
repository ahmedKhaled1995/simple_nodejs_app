pipeline {
    agent any

    stages {
        
        stage('Pukking Repo Files') {
            steps {
              git branch: "${GIT_BRANCH}", credentialsId: 'github', url: 'https://github.com/ahmedKhaled1995/simple_nodejs_app.git'
            }
        }
        
        stage('Stage 1') {
            steps {
                sh ''' 
                    ls
                    cal
                '''
            }
        }
        
    }
}
