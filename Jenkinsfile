pipeline {
    agent { docker { image 'python:3.5.1' } }

    environment {
        AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
        AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
    }
    stages {
        stage('Credentials Stage') {
            steps {
                sh 'echo $AWS_ACCESS_KEY_ID'
		sh 'echo $AWS_SECRET_ACCESS_KEY' 
            }
        }
    }
}
