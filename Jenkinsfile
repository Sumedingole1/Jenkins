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
                        sh 'export MAVEN_HOME=/opt/apache-maven-3.8.7/'
                        sh 'export JAVA_HOME=/opt/jdk-17.0.4.1+1/'
                        sh 'export PATH=${MAVEN_HOME}/bin:${JAVA_HOME}/bin:${PATH}'

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
