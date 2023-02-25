pipeline {
    agent {
        label 'jdk17'
    }
    tools {
        maven 'maven-3.9.0'
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn verify'
            }
        }
    }
}
