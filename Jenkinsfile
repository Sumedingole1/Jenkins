pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'pwd'
                sh 'ls -l'
                
                script {
                    dir('/var/lib/jenkins/workspace/Samle') {
                        sh 'mvn clean'
                    }
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                // Add your test steps here
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
