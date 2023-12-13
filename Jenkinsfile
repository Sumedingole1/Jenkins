pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ls -l'
                script {
                    dir('/var/lib/jenkins/workspace/Samle') {
                        sh '/opt/apache-maven-3.8.7/bin/mvn clean'
                    }
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh '/opt/apache-maven-3.8.7/bin/mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                // Add your deployment steps here
                sh 'rm -rf /var/lib/jenkins/workspace/*'
            }
        }
    }
}
