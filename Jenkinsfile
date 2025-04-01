pipeline {
    agent any
    //tools {
    //    maven 'maven'  // Ensure this matches the Maven tool name configured in Jenkins
    //}
    stages {
        stage("Git checkout") {
            steps {
                git 'https://github.com/sten-benny/Maven-Web-Project.git'
            }
        }
        stage("Unit test") {
            steps {
                sh 'mvn --version'  // Check if Maven is installed
                sh 'mvn test'
            }
        }
    }
}
