pipeline {
    agent ssh-aws

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ls -l'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                // Add your deployment steps here
            }
        }
    }
}
