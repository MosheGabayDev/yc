pipeline {
    agent any
    environment {
		DOCKERHUB_CREDENTIALS=credentials('DockerHub')
	}
    stages {
        stage('Build'){
            steps {
                sh """
                    ls
                    pwd
                    docker build -t my-nginx-test:1 .
                    echo $DOCKERHUB_CREDENTIALS
                """
            }
        }

    }
}