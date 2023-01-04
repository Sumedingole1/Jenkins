pipeline {
    agent any
    
    tools {
        maven 'Maven 3.8.7'
    }

    stages {
        stage ('Initialize') {
            steps {
                yum install java-11-openjdk-devel -y 
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                
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
            }
        }
    }
}
