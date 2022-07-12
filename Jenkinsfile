pipeline {
    agent any
    environment {
        AWS_DEFAULT_REGION="us-east-1"
    }
    stages {
        stage('Build'){
            steps {
                sh """
                    ls
                    pwd
                """
                withCredentials([aws(
                    credentialsId: 'private',
                    accessKeyVariable: 'AWS_ACCESS_KEY_ID',
                    secretKeyVariable: 'AWS_SECRET_ACCESS_KEY'
                )]) {
                    sh '''
                        
                    '''
                }

            }
        }

    }
}