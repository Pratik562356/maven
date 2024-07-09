pipeline {
    agent any

    tools {
        maven 'maven' // Name of the Maven installation configured in Jenkins
         // Name of the JDK installation configured in Jenkins
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
    
