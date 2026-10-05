pipeline {
    agent any
    environment {
        JAVA_HOME = 'C:\\Program Files\\Eclipse Adoptium\\jdk-21'
        PATH = "C:\\Program Files\\Eclipse Adoptium\\jdk-21\\bin;C:\\Users\\aryaa\\.m2\\wrapper\\dists\\apache-maven-3.6.3-bin\\1iopthnavndlasol9gbrbg6bf2\\apache-maven-3.6.3\\bin;C:\\Program Files\\Git\\bin;C:\\Program Files\\Git\\cmd;${env.PATH}"
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/aryaanand055/Jenkins-CI-Demo.git'
            }
        }
        stage('Build and Test') {
            steps {
                sh 'mvn clean test'
            }
        }
    }
}
