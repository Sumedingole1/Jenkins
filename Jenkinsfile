pipeline {
    agent any
    
    tools {
        maven 'Maven 3.8.7'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                wget https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz /opt
                cd /opt
                ls -l
                
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
