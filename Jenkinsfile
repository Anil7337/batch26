pipeline {
    agent any

    tools {
        maven 'Maven 3.8.1' // Must be configured in Jenkins > Global Tool Configuration
        jdk 'JDK 11'        // Ensure JDK is installed and configured
    }

    environment {
        BRANCH_NAME = "${env.BRANCH_NAME}"
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Cloning source from branch: ${env.BRANCH_NAME}"
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building the project on branch: ${env.BRANCH_NAME}"
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                echo "Packaging the application..."
                sh 'mvn package'
            }
        }
    }

   
