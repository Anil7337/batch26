pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning GitHub Repository...'
                
            }
        }

        stage('Build') {
            steps {
                echo 'Compiling Java code...'
                sh 'javac HelloWorld.java'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging application...'
                
            }
        }
    }
}
