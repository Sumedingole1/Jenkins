pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'pwd'
                sh 'ls -l'
                sh '/opt/apache-maven-3.8.7/bin/mvn -v'
                
                script {
                    dir('/var/lib/jenkins/workspace/Samle') {
                        sh '/opt/apache-maven-3.8.7/bin/mvn clean'
                        sh 'ls -l'
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
