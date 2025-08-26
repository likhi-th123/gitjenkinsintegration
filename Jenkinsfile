pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Pull code from Git repository
                git branch: 'master', url: 'https://github.com/likhi-th123/gitjenkinsintegration.git'
            }
        }
        stage('Compile') {
            steps {
                // Compile Java code
                bat 'javac Sample.java'
            }
        }
        stage('Run Main and Tests') {
            steps {
                // Run main method (which calls testMethod)
                bat 'java Sample'
            }
        }
    }
}