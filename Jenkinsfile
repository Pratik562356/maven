pipeline {
    agent any

    tools {
        maven 'maven' // Name of the Maven installation configured in Jenkins
         // Name of the JDK installation configured in Jenkins
    }

    

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/Pratik562356/maven.git', branch: 'main'
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

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
    
