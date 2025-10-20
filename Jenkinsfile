pipeline {
    agent any
    tools {
        jdk 'JDK17'
    }
    stages {
        stage('Checkout code')
        {
            steps {
                git branch: 'master', url: 'https://github.com/GharbiAmal/Git-exemple.git'
            }
        }
        stage('Compile code')
        {
            steps {
                sh 'javac src/application/Test.java'
            }
        }
        stage('Execute code')
        {
            steps {
                sh 'java -cp src application.Test'
            }
        }
        stage('display message')
        {
            steps {
                echo 'Hello from github
            }
        }
    }
}
