pipeline {
    agent any
    tools {
        maven 'maven-3.8'  // ou le nom de ton Maven dans Jenkins
        jdk 'jdk17'
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/1malek/student-management.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
