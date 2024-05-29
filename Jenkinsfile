pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Compiling the Java program
                sh 'javac -d build src/HelloWorld.java'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Running the compiled Java program
                sh 'java -cp build src.HelloWorld'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Deployment steps go here
            }
        }
    }
}
