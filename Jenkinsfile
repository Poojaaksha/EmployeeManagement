pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'dotnet build EmployeeManagement.sln'
            }
        }

        stage('Test') {
            steps {
                sh 'dotnet test EmployeeManagement.sln'
            }
        }

    }
}
