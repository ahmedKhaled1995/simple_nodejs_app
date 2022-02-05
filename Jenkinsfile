pipeline {
    agent { label 'Slave-machine1' }

    stages {
       
        stage('Stage 1') {
            steps {
                sh ''' 
                echo omar fandoud
                    ls
                    
                '''
            }
        }
        
    }
    post {
        always{
        slackSend color: "good", message: "Message from Jenkins Pipeline"
        }
    }
}
