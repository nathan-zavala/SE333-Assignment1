pipeline {
    agent any

    tools {
        // These names MUST match the tools you configured in Jenkins
        maven 'M3'
        jdk   'JDK11'
    }

    stages {
        stage('Checkout') {
            steps {
                // Uses the repo Jenkins is pointed at (your SE333-Assignment1 repo)
                checkout scm
            }
        }

        stage('Build') {
            steps {
                // Build / compile the project
                sh 'mvn -B clean compile'
            }
        }

        stage('Test') {
            steps {
                // Run tests
                sh 'mvn -B test'

                // Publish JUnit test results (so Jenkins can show test reports)
                junit '**/target/surefire-reports/*.xml'
            }
        }
    }
}
