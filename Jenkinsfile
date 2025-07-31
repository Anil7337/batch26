pipeline {
    agent any

    tools {
        maven 'Maven 3.8.1' 
        jdk 'JDK 11'        
    }

    
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Cloning source from branch: ${env.BRANCH_NAME}"
                
            }
        }

        stage('Build') {
            steps {
                echo "Building the project on branch: ${env.BRANCH_NAME}"
                
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                
            }
        }

        stage('Package') {
            steps {
                echo "Packaging the application..."
                
            }
        }
    }

    
