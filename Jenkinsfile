pipeline {
    agent any

    environment {
        JAVA_HOME = 'C:\\Program Files\\Java\\jdk-21'
        PATH = "${env.JAVA_HOME}\\bin;${env.PATH}"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/madhuk54/pr4.git'
            }
        }

        stage('Compile') {
            steps {
                bat 'javac pract.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java  pract.java'
            }
        }
    }
}
